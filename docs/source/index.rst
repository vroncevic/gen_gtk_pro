GEN_GTK_PRO
------------

.. toctree::
 :hidden:

 self

gen_gtk_pro is shell tool for generating GTK project.

Developed in bash code: 100%.

The README is used to introduce the tool and provide instructions on
how to install the tool, any machine dependencies it may have and any
other information that should be provided before the tool is installed.

|GitHub issues| |Documentation Status| |GitHub contributors|

.. |GitHub issues| image:: https://img.shields.io/github/issues/vroncevic/gen_gtk_pro.svg
   :target: https://github.com/vroncevic/gen_gtk_pro/issues

.. |GitHub contributors| image:: https://img.shields.io/github/contributors/vroncevic/gen_gtk_pro.svg
   :target: https://github.com/vroncevic/gen_gtk_pro/graphs/contributors

.. |Documentation Status| image:: https://readthedocs.org/projects/gen_gtk_pro/badge/?version=latest
   :target: https://gen_gtk_pro.readthedocs.io/projects/gen_gtk_pro/en/latest/?badge=latest

INSTALLATION
-------------
Navigate to release `page`_ download and extract release archive.

.. _page: https://github.com/vroncevic/gen_gtk_pro/releases

To install this set of modules type the following:

.. code-block:: bash

   tar xvzf gen_gtk_pro-x.y.z.tar.gz
   cd gen_gtk_pro-x.y.z
   cp -R ~/sh_tool/bin/   /root/scripts/gen_gtk_pro/ver.1.0/
   cp -R ~/sh_tool/conf/  /root/scripts/gen_gtk_pro/ver.1.0/
   cp -R ~/sh_tool/log/   /root/scripts/gen_gtk_pro/ver.1.0/

DEPENDENCIES
-------------
This tool requires these other modules and libraries:

.. code-block:: bash

   sh_util https://github.com/vroncevic/sh_util

SHELL TOOL STRUCTURE
---------------------
gen_gtk_pro is based on MOP.

Shell tool structure:

.. code-block:: bash

   .
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

COPYRIGHT AND LICENCE
----------------------

|License: GPL v3| |License: Apache 2.0|

.. |License: GPL v3| image:: https://img.shields.io/badge/License-GPLv3-blue.svg
   :target: https://www.gnu.org/licenses/gpl-3.0

.. |License: Apache 2.0| image:: https://img.shields.io/badge/License-Apache%202.0-blue.svg
   :target: https://opensource.org/licenses/Apache-2.0

Copyright (C) 2018 by https://vroncevic.github.io/gen_gtk_pro

This tool is free software; you can redistribute it and/or modify it
under the same terms as Bash itself, either Bash version 4.2.47 or,
at your option, any later version of Bash 4 you may have available.

