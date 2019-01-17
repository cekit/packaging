# Cekit packaging

This repository contains all the Cekit packaging related information. Currently it's holding RPM spec files for our [copr repositories](https://copr.fedorainfracloud.org/coprs/g/cekit/cekit/).

For information on how to install Cekit, please refer to the [upstream documentation](https://cekit.readthedocs.io/en/latest/installation.html).

## Spec files

In the `rpms` directory you can find spec files used to build Cekit-related RPM files. Below you can find information what files are located in this directory and why.

### `python-cekit.spec`

Main Cekit spec file. Provides the RPM for latest stable release.

### `python-cekit-next.spec`

Development package. Provides Cekit from the `develop` branch. This package is built on-demand.

### `python-pykwalify.spec`

Updated [pyKwalify](https://github.com/grokzen/pykwalify) package. The currently shipped (in Fedora and EPEL too) is at version 1.5, but we [require 1.6+](https://github.com/Grokzen/pykwalify/releases).

### `python-docopt.spec`

Package required by the Python Kwalify library. Required only for CentOS/RHEL. Fedora provides this package.

### `python-colorlog.spec`

As the name suggest, used to provide colorful output of logs. Very useful. Used only for CentOS/RHEL. Fedora provides this package.
