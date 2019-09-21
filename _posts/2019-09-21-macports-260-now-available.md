---
title: MacPorts 2.6.0 now available
slug: macports-260-now-available
date: 2019-09-21 02:54:04
---

The MacPorts Project is happy to announce that the 2.6.0 version has now
been released. It is available via the usual methods:

- selfupdate if you already have MacPorts installed
- package installers for [10.14][1], [10.13][2], [10.12][3], [10.11][4], [10.10][5], [10.9][6],
[10.8][7], [10.7][8], [10.6][9], [10.5][10] and [10.4][11] (universal i386/ppc for 10.5 and 10.4,
i386/x86\_64 for 10.6, and the rest x86\_64)
- source tarballs, both [.tar.bz2][12] and [.tar.gz][13]
- [git tag][14]

The list of what's new in 2.6.0 can be found in the [ChangeLog][15].

Of special note for users of 10.6-10.8: The default C++ stdlib has changed from
libstdc++ to libc++. This will enable building ports that require C++11
and beyond much more easily. All C++-based ports using the old stdlib
will need to be rebuilt, so we recommend that you run 'sudo port
rev-upgrade' after installing the beta.

We are currently in the process of switching the packages server over
to the new stdlib, so availability of binary packages
for 10.6-10.8 will be reduced for a time until the builds catch up.
(There will initially be no availability for a hopefully very short time
until we flip the switch to mark the archives as libc++.)

If you previously followed the LibcxxOnOlderSystems instructions on the
wiki, you should revert the changes to macports.conf that the
instructions specify. In particular, default_compilers should not be set
so that the new MacPorts version can pick the compilers itself. You also
probably want buildfromsource to be its default value ("ifneeded") so
that you will use binaries once they are available.

A big thanks to the developers for their hard work with all of the
various features and bug fixes in 2.6.0, and to all those who helped out
by reporting bugs or testing.

Detached PGP signatures for the pkg/dmgs and source tarballs have been
made by Joshua Root, whose public key is available on the keyservers and the
[MacPorts wiki][16].

Key ID: 0x01FF673FB4AAE6CD  
Fingerprint: C403 7936 5723 6DCF 2E58  0C02 01FF 673F B4AA E6CD

The MacPorts Port Managers

[1]: <https://github.com/macports/macports-base/releases/download/v2.6.0/MacPorts-2.6.0-10.14-Mojave.pkg>
[2]: <https://github.com/macports/macports-base/releases/download/v2.6.0/MacPorts-2.6.0-10.13-HighSierra.pkg>
[3]: <https://github.com/macports/macports-base/releases/download/v2.6.0/MacPorts-2.6.0-10.12-Sierra.pkg>
[4]: <https://github.com/macports/macports-base/releases/download/v2.6.0/MacPorts-2.6.0-10.11-ElCapitan.pkg>
[5]: <https://github.com/macports/macports-base/releases/download/v2.6.0/MacPorts-2.6.0-10.10-Yosemite.pkg>
[6]: <https://github.com/macports/macports-base/releases/download/v2.6.0/MacPorts-2.6.0-10.9-Mavericks.pkg>
[7]: <https://github.com/macports/macports-base/releases/download/v2.6.0/MacPorts-2.6.0-10.8-MountainLion.pkg>
[8]: <https://github.com/macports/macports-base/releases/download/v2.6.0/MacPorts-2.6.0-10.7-Lion.pkg>
[9]: <https://github.com/macports/macports-base/releases/download/v2.6.0/MacPorts-2.6.0-10.6-SnowLeopard.pkg>
[10]: <https://github.com/macports/macports-base/releases/download/v2.6.0/MacPorts-2.6.0-10.5-Leopard.dmg>
[11]: <https://github.com/macports/macports-base/releases/download/v2.6.0/MacPorts-2.6.0-10.4-Tiger.dmg>
[12]: <https://github.com/macports/macports-base/releases/download/v2.6.0/MacPorts-2.6.0.tar.bz2>
[13]: <https://github.com/macports/macports-base/releases/download/v2.6.0/MacPorts-2.6.0.tar.gz>
[14]: <https://github.com/macports/macports-base/releases/tag/v2.6.0>
[15]: <https://github.com/macports/macports-base/blob/v2.6.0/ChangeLog>
[16]: <https://trac.macports.org/wiki/jmr>
