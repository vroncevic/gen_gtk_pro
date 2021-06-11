<img align="right" src="https://raw.githubusercontent.com/vroncevic/gen_gtk_pro/dev/docs/gen_gtk_pro_logo.png" width="25%">

# Generate GTK C Project

**gen_gtk_pro** is shell tool for generating GTK C project.

Developed in **[bash](https://en.wikipedia.org/wiki/Bash_(Unix_shell))** code: **100%**.

[![gen_gtk_pro shell checker](https://github.com/vroncevic/gen_gtk_pro/workflows/gen_gtk_pro%20shell%20checker/badge.svg)](https://github.com/vroncevic/gen_gtk_pro/actions?query=workflow%3A%22gen_gtk_pro+shell+checker%22)

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

Navigate to release **[page](https://github.com/vroncevic/gen_gtk_pro/releases)** download and extract release archive.

To install **gen_gtk_pro** type the following:

```
tar xvzf gen_gtk_pro-x.y.tar.gz
cd gen_gtk_pro-x.y
cp -R ~/sh_tool/bin/   /root/scripts/gen_gtk_pro/ver.x.y/
cp -R ~/sh_tool/conf/  /root/scripts/gen_gtk_pro/ver.x.y/
cp -R ~/sh_tool/log/   /root/scripts/gen_gtk_pro/ver.x.y/
```

![alt tag](https://raw.githubusercontent.com/vroncevic/gen_gtk_pro/dev/docs/setup_tree.png)

Or You can use docker to create image/container.

[![gen_gtk_pro docker checker](https://github.com/vroncevic/gen_gtk_pro/workflows/gen_gtk_pro%20docker%20checker/badge.svg)](https://github.com/vroncevic/gen_gtk_pro/actions?query=workflow%3A%22gen_gtk_pro+docker+checker%22)

### Usage

```
# Create symlink for shell tool
ln -s /root/scripts/gen_gtk_pro/ver.x.y/bin/gen_gtk_pro.sh /root/bin/gen_gtk_pro

# Setting PATH
export PATH=${PATH}:/root/bin/

# Generating GTK C project
gen_gtk_pro SimpleTest
```

### Dependencies

**gen_gtk_pro** requires next modules and libraries:
* sh_util [https://github.com/vroncevic/sh_util](https://github.com/vroncevic/sh_util)

### Shell tool structure

**gen_gtk_pro** is based on MOP.

Code structure:
```
sh_tool/
├── bin/
│   └── gen_gtk_pro.sh
├── conf/
│   ├── gen_gtk_pro.cfg
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

[![Documentation Status](https://readthedocs.org/projects/gen_gtk_pro/badge/?version=latest)](https://gen_gtk_pro.readthedocs.io/projects/gen_gtk_pro/en/latest/?badge=latest)

More documentation and info at:
* [https://gen_gtk_pro.readthedocs.io/en/latest/](https://gen_gtk_pro.readthedocs.io/en/latest/)
* [https://www.gnu.org/software/bash/manual/](https://www.gnu.org/software/bash/manual/)
* [https://developer.gnome.org/gtk3](https://developer.gnome.org/gtk3/stable/gtk-getting-started.html)

### Copyright and licence

[![License: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0) [![License](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)

Copyright (C) 2017 by [vroncevic.github.io/gen_gtk_pro](https://vroncevic.github.io/gen_gtk_pro)

**gen_gtk_pro** is free software; you can redistribute it and/or modify
it under the same terms as Bash itself, either Bash version 4.2.47 or,
at your option, any later version of Bash 4 you may have available.

Lets help and support FSF.

[![Free Software Foundation](https://raw.githubusercontent.com/vroncevic/gen_gtk_pro/dev/docs/fsf-logo_1.png)](https://my.fsf.org/)

[![Donate](https://www.paypalobjects.com/en_US/i/btn/btn_donateCC_LG.gif)](https://my.fsf.org/donate/)
