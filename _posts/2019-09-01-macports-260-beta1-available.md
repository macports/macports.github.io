---
title: MacPorts 2.6.0 beta1 available
slug: macports-260-beta1-available
date: 2019-09-01 16:34:45
---

Source code and pkgs for MacPorts 2.6.0-beta1 are now
[available][1]. Testing of either of these install methods is helpful.

Be prepared to encounter bugs. As always, having a recent backup would
be wise. Please [report][2] any bugs that you find (after first [searching
Trac][3], of course!)

There are a large number of changes in this release. See the [ChangeLog][4]
for a list of most of the major ones. You may like to focus your
testing on the new features in that list, as well as your normal usage.

Of special note:

 * For 10.14 users: The pkg meets Apple's new requirements for
notarization. This includes enabling the hardened runtime for all
executables, which has the potential to cause new issues due to denying
access to certain system resources and preventing the loading of
unsigned plugins. Please let us know about any such problems.

 * For users of 10.6-10.8: The default C++ stdlib has changed from
libstdc++ to libc++. This will enable building ports that require C++11
and beyond much more easily. All C++-based ports using the old stdlib
will need to be rebuilt, so we recommend that you run 'sudo port
rev-upgrade' after installing the beta.

 You will no longer get binary packages for 10.6-10.8 until we switch the
packages server over to the new stdlib along with the final 2.6.0
release. You may want to install clang-8.0, clang-3.7, clang-3.4 and
their dependencies before installing the beta, to save a bit of build
time (the newer clang versions already use libc++ and so won't need to
be rebuilt.)

 If you previously followed the LibcxxOnOlderSystems instructions on the
wiki, you should revert the changes to macports.conf that the
instructions specify. In particular, default_compilers should not be set
so that the new MacPorts version can pick the compilers itself. You also
probably want buildfromsource to be its default value ("ifneeded") so
that you will use binaries once they are available.

[1]: https://github.com/macports/macports-base/releases/tag/v2.6.0-beta1
[2]: https://trac.macports.org/newticket
[3]: https://trac.macports.org/search
[4]: https://github.com/macports/macports-base/blob/release-2.6/ChangeLog
