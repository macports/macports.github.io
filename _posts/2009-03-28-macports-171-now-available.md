---
title: MacPorts 1.7.1 now available
slug: macports-171-now-available
permalink: /post/macports-171-now-available
date: 2009-03-28 18:34:46.269197-07
---

The MacPorts Project is proud to announce the release of version 1.7.1. This is a bugfix release with small changes only.

Notable changes for end users:

* port upgrade will no longer act on ports which are not installed

Notable changes for port authors:

* port lint no longer requires `master_sites` if the port does not have any distfiles
* `${applications_dir}` and `${frameworks_dir}` are automatically created in the destroot
* `configure.compiler` supports apple-gcc-4.2
* New `use_7z yes` port option to allow distfiles in 7z format

If you already have MacPorts installed, the preferred method for updating is to run:

    sudo port selfupdate

For new installs, there are also [package installers](https://svn.macports.org/repository/macports/downloads/MacPorts-1.7.1/) in disk images available for 10.3, 10.4, and 10.5 (with the latter two being universal builds). The source is available as tarballs compressed with gzip or bzip2 in the same directory and it is also available from the [subversion tag](https://svn.macports.org/repository/macports/tags/release_1_7_1/).

You can also read the [email announcement](https://lists.macosforge.org/pipermail/macports-announce/2009-March/000003.html).
