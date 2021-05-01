---
title: MacPorts 2.7.0 beta2 available
slug: macports-270-beta2-available
date: 2021-05-01 09:54:59
---

Source code and pkgs for MacPorts 2.7.0-beta2 are now
[available][1]. Testing of either of these install methods is helpful.

Be prepared to encounter bugs. As always, having a recent backup would
be wise. Please [report][2] any bugs that you find (after first [searching
Trac][3], of course!)

There are a large number of changes in this release. See the [ChangeLog][4]
for a list of most of the major ones. You may like to focus your
testing on the new features in that list, as well as your normal usage.

Notable changes since beta1 are:
 * Fixed an error that could occur when applying the previously requested variants when upgrading. ([#62751][5])
 * Fixed progress bar width when COLUMNS is not set in the environment.
 * Fixed inability to read the registry database without write permission when using newer SQLite versions.

Known issue: The change committed as [4f276ab][6] needs to be applied on
10.6 and older to successfully build base against the system SQLite.

[1]: https://github.com/macports/macports-base/releases/tag/v2.7.0-beta2
[2]: https://trac.macports.org/newticket
[3]: https://trac.macports.org/search
[4]: https://github.com/macports/macports-base/blob/release-2.7/ChangeLog
[5]: https://trac.macports.org/ticket/62751
[6]: https://github.com/macports/macports-base/commit/4f276ab2335e02a4bc6badca8f96eacf6f2f0de5
