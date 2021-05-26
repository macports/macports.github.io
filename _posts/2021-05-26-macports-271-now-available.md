---
title: MacPorts 2.7.1 now available
slug: macports-271-now-available
date: 2021-05-26 13:42:26
---

The MacPorts Project is pleased to announce the release of version
2.7.1. This is a bugfix release with small changes only. See the
[ChangeLog][1] for the list of changes.

If you already have MacPorts installed, the preferred method for
updating is to run:

    sudo port selfupdate

For new installs, [package installers][2] are available for the most current
macOS 11 Big Sur and all older releases back to Mac OS X 10.4 Tiger. The
source is also available as tarballs compressed with gzip or bzip2, or from the
[git tag][3].

Note for macOS 10.14 users: if you are unable to selfupdate due to the
SQL error mentioned in the ChangeLog, you will need to install
MacPorts 2.7.1 either with the .pkg installer or from source.

Detached PGP signatures for the disk images, package installers and
source tarballs have been made by [Joshua Root][4], and the git tag has
been signed with the same key. The public key is available on the
keyservers and the MacPorts wiki, the fingerprint being:

0x01FF673FB4AAE6CD: C403 7936 5723 6DCF 2E58  0C02 01FF 673F B4AA E6CD

The MacPorts Port Managers

[1]: <https://github.com/macports/macports-base/blob/release-2.7/ChangeLog>
[2]: <https://www.macports.org/install.php>
[3]: <https://github.com/macports/macports-base/releases/tag/v2.7.1>
[4]: <https://trac.macports.org/wiki/jmr>
