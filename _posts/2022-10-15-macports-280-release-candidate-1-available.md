---
title: MacPorts 2.8.0 release candidate 1 available
slug: macports-280-release-candidate-1-available
date: 2022-10-15 21:18:05
---

Source code and pkgs for MacPorts 2.8.0-rc1 are now
[available][1]. Testing of either of these install methods is helpful.

Be prepared to encounter bugs. As always, having a recent backup would
be wise. Please [report][2] any bugs that you find (after first [searching
Trac][3], of course!)

If no show-stopping bugs are found in the next few days, this will
become the 2.8.0 release.

There are a large number of changes in this release. See the [ChangeLog][4]
for a list of most of the major ones. You may like to focus your
testing on the new features in that list, as well as your normal usage.

Changes since beta1 are:
 * Fixed error when upgrading ports with no cxx_stdlib information in the registry.
 * Ensured that SQLite write-ahead logging is enabled on all systems.

[1]: https://github.com/macports/macports-base/releases/tag/v2.8.0-rc1
[2]: https://trac.macports.org/newticket
[3]: https://trac.macports.org/search
[4]: https://github.com/macports/macports-base/blob/release-2.8/ChangeLog
