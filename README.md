<img align="right" src="https://raw.githubusercontent.com/vroncevic/gen_gtk_pro/dev/docs/gen_gtk_pro_logo.png" width="25%">

# Generate GTK C Project

**gen_gtk_pro** is shell tool for generating GTK C project.

Developed in **[bash](https://en.wikipedia.org/wiki/Bash_(Unix_shell))** code: **100%**.

[![gen_gtk_pro_shell_checker](https://github.com/vroncevic/gen_gtk_pro/actions/workflows/gen_gtk_pro_shell_checker.yml/badge.svg)](https://github.com/vroncevic/gen_gtk_pro/actions/workflows/gen_gtk_pro_shell_checker.yml)

The README is used to introduce the modules and provide instructions on
how to install the modules, any machine dependencies it may have and any
other information that should be provided before the modules are installed.

[![GitHub issues open](https://img.shields.io/github/issues/vroncevic/gen_gtk_pro.svg)](https://github.com/vroncevic/gen_gtk_pro/issues) [![GitHub contributors](https://img.shields.io/github/contributors/vroncevic/gen_gtk_pro.svg)](https://github.com/vroncevic/gen_gtk_pro/graphs/contributors)

<!-- START doctoc generated TOC please keep comment here to allow auto update -->
<!-- DON'T EDIT THIS SECTION, INSTEAD RE-RUN doctoc TO UPDATE -->
**Table of Contents**

- [Installation](#installation)
- [Usage](#usage)
- [Dependencies](#dependencies)
- [Shell tool structure](#shell-tool-structure)
- [Docs](#docs)
- [Copyright and licence](#copyright-and-licence)

<!-- END doctoc generated TOC please keep comment here to allow auto update -->

### Installation

![Debian Linux OS](https://raw.githubusercontent.com/vroncevic/gen_gtk_pro/dev/docs/debtux.png)

Navigate to release **[page](https://github.com/vroncevic/gen_gtk_pro/releases)** download and extract release archive.

To install **gen_gtk_pro** type the following

```
tar xvzf gen_gtk_pro-x.y.tar.gz
cd gen_gtk_pro-x.y
cp -R ~/sh_tool/bin/   /root/scripts/gen_gtk_pro/ver.x.y/
cp -R ~/sh_tool/conf/  /root/scripts/gen_gtk_pro/ver.x.y/
cp -R ~/sh_tool/log/   /root/scripts/gen_gtk_pro/ver.x.y/
```

Self generated setup script and execution
```
./gen_gtk_pro_setup.sh 

[setup] installing App/Tool/Script gen_gtk_pro
	Sun 05 Dec 2021 05:57:06 PM CET
[setup] copy App/Tool/Script structure
[setup] remove github editor configuration files
[setup] set App/Tool/Script permission
[setup] create symbolic link of App/Tool/Script
[setup] done

/root/scripts/gen_gtk_pro/ver.2.0/
├── bin/
│   ├── center.sh
│   ├── display_logo.sh
│   └── gen_gtk_pro.sh
├── conf/
│   ├── gen_gtk_pro.cfg
│   ├── gen_gtk_pro.logo
│   ├── gen_gtk_pro_util.cfg
│   ├── project_set.cfg
│   └── template/
│       ├── authors.template
│       ├── autogen.template
│       ├── c_editorconfig.template
│       ├── changelog.template
│       ├── configure_ac.template
│       ├── copying.template
│       ├── c_source.template
│       ├── makefile_am_root.template
│       ├── makefile_am_src.template
│       ├── news.template
│       ├── readme.template
│       └── ui.template
└── log/
    └── gen_gtk_pro.log

4 directories, 20 files
lrwxrwxrwx 1 root root 52 Dec  5 17:57 /root/bin/gen_gtk_pro -> /root/scripts/gen_gtk_pro/ver.2.0/bin/gen_gtk_pro.sh
```

Or You can use docker to create image/container.

### Usage

```
# Create symlink for shell tool
ln -s /root/scripts/gen_gtk_pro/ver.x.y/bin/gen_gtk_pro.sh /root/bin/gen_gtk_pro

# Setting PATH
export PATH=${PATH}:/root/bin/

# Generating GTK C project
gen_gtk_pro rcp

gen_gtk_pro ver.2.0
Sun 05 Dec 2021 05:58:55 PM CET

[check_root] Check permission for current session? [ok]
[check_root] Done

                                                                                       
                                            ██   ██                                    
                                           ░██  ░██                                    
    █████   █████  ███████         █████  ██████░██  ██       ██████  ██████  ██████   
   ██░░░██ ██░░░██░░██░░░██       ██░░░██░░░██░ ░██ ██       ░██░░░██░░██░░█ ██░░░░██  
  ░██  ░██░███████ ░██  ░██      ░██  ░██  ░██  ░████        ░██  ░██ ░██ ░ ░██   ░██  
  ░░██████░██░░░░  ░██  ░██      ░░██████  ░██  ░██░██       ░██████  ░██   ░██   ░██  
   ░░░░░██░░██████ ███  ░██ █████ ░░░░░██  ░░██ ░██░░██ █████░██░░░  ░███   ░░██████   
    █████  ░░░░░░ ░░░   ░░ ░░░░░   █████    ░░  ░░  ░░ ░░░░░ ░██     ░░░     ░░░░░░    
   ░░░░░                          ░░░░░                      ░░                        
                                                                                        
	                                                     
		Info   github.io/gen_gtk_pro ver.2.0 
		Issue  github.io/issue
		Author vroncevic.github.io

[gen_gtk_pro] Loading basic and util configuration!
100% [================================================]

[load_conf] Loading App/Tool/Script configuration!
[check_cfg] Checking configuration file [/root/scripts/gen_gtk_pro/ver.2.0/conf/gen_gtk_pro.cfg] [ok]
[check_cfg] Done

[load_conf] Done

[load_util_conf] Load module configuration!
[check_cfg] Checking configuration file [/root/scripts/gen_gtk_pro/ver.2.0/conf/gen_gtk_pro_util.cfg] [ok]
[check_cfg] Done

[load_util_conf] Done

[load_util_conf] Load module configuration!
[check_cfg] Checking configuration file [/root/scripts/gen_gtk_pro/ver.2.0/conf/project_set.cfg] [ok]
[check_cfg] Done

[load_util_conf] Done

[gen_gtk_pro] Generate project structure!
[gen_gtk_pro] Generating directory [/data/dev/bash/3_tools/gen_gtk_pro/rcp/]
[gen_gtk_pro] Generating file [/data/dev/bash/3_tools/gen_gtk_pro/rcp/autogen.sh]
[gen_gtk_pro] Generating file [/data/dev/bash/3_tools/gen_gtk_pro/rcp/configure.ac]
[gen_gtk_pro] Generating directory [/data/dev/bash/3_tools/gen_gtk_pro/rcp/po/]
[gen_gtk_pro] Generating file [/data/dev/bash/3_tools/gen_gtk_pro/rcp/po/ChangeLog]
[gen_gtk_pro] Generating file [/data/dev/bash/3_tools/gen_gtk_pro/rcp/po/LINGUAS]
[gen_gtk_pro] Generate file [/data/dev/bash/3_tools/gen_gtk_pro/rcp/po/POTFILES.in]
[gen_gtk_pro] Generating directory [/data/dev/bash/3_tools/gen_gtk_pro/rcp/src/]
[gen_gtk_pro] Generating file [/data/dev/bash/3_tools/gen_gtk_pro/rcp/src/main.c]
[gen_gtk_pro] Generating file [/data/dev/bash/3_tools/gen_gtk_pro/rcp/src/.editorconfig]
[gen_gtk_pro] Generating file [/data/dev/bash/3_tools/gen_gtk_pro/rcp/src/rcp.ui]
[gen_gtk_pro] Generating file [/data/dev/bash/3_tools/gen_gtk_pro/rcp/src/Makefile.am]
[gen_gtk_pro] Generating file [/data/dev/bash/3_tools/gen_gtk_pro/rcp/Makefile.am]
[gen_gtk_pro] Generating file [/data/dev/bash/3_tools/gen_gtk_pro/rcp/COPYING]
[gen_gtk_pro] Generating file [/data/dev/bash/3_tools/gen_gtk_pro/rcp/AUTHORS]
[gen_gtk_pro] Generating file [/data/dev/bash/3_tools/gen_gtk_pro/rcp/NEWS]
[gen_gtk_pro] Generating file [/data/dev/bash/3_tools/gen_gtk_pro/rcp/README]
[gen_gtk_pro] Set permission!
[gen_gtk_pro] Set permission!
[logging] Checking directory [/root/scripts/gen_gtk_pro/ver.2.0/log/]? [ok]
[logging] Write info log!
[logging] Done

[gen_gtk_pro] Done

[check_tool] Checking tool [/usr/bin/tree]? [ok]
[check_tool] Done

/data/dev/bash/3_tools/gen_gtk_pro/rcp/
├── AUTHORS
├── autogen.sh
├── ChangeLog
├── configure.ac
├── COPYING
├── Makefile.am
├── NEWS
├── po
│   ├── ChangeLog
│   ├── LINGUAS
│   └── POTFILES.in
├── README
└── src
    ├── main.c
    ├── Makefile.am
    └── rcp.ui

2 directories, 14 files
```

### Dependencies

**gen_gtk_pro** requires next modules and libraries
* sh_util [https://github.com/vroncevic/sh_util](https://github.com/vroncevic/sh_util)

### Shell tool structure

**gen_gtk_pro** is based on MOP.

Shell tool structure
```
sh_tool/
├── bin/
│   ├── center.sh
│   ├── display_logo.sh
│   └── gen_gtk_pro.sh
├── conf/
│   ├── gen_gtk_pro.cfg
│   ├── gen_gtk_pro.logo
│   ├── gen_gtk_pro_util.cfg
│   ├── project_set.cfg
│   └── template/
│       ├── authors.template
│       ├── autogen.template
│       ├── c_editorconfig.template
│       ├── changelog.template
│       ├── configure_ac.template
│       ├── copying.template
│       ├── c_source.template
│       ├── makefile_am_root.template
│       ├── makefile_am_src.template
│       ├── news.template
│       ├── readme.template
│       └── ui.template
└── log/
    └── gen_gtk_pro.log
```

### Docs

[![Documentation Status](https://readthedocs.org/projects/gen_gtk_pro/badge/?version=latest)](https://gen-gtk-pro.readthedocs.io/projects/gen_gtk_pro/en/latest/?badge=latest)

More documentation and info at
* [https://gen_gtk_pro.readthedocs.io/en/latest/](https://gen-gtk-pro.readthedocs.io/en/latest/)
* [https://www.gnu.org/software/bash/manual/](https://www.gnu.org/software/bash/manual/)
* [https://developer.gnome.org/gtk3](https://developer.gnome.org/gtk3/stable/gtk-getting-started.html)

### Copyright and licence

[![License: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0) [![License](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)

Copyright (C) 2017 - 2024 by [vroncevic.github.io/gen_gtk_pro](https://vroncevic.github.io/gen_gtk_pro)

**gen_gtk_pro** is free software; you can redistribute it and/or modify
it under the same terms as Bash itself, either Bash version 4.2.47 or,
at your option, any later version of Bash 4 you may have available.

Lets help and support FSF.

[![Free Software Foundation](https://raw.githubusercontent.com/vroncevic/gen_gtk_pro/dev/docs/fsf-logo_1.png)](https://my.fsf.org/)

[![Donate](https://www.paypalobjects.com/en_US/i/btn/btn_donateCC_LG.gif)](https://my.fsf.org/donate/)
