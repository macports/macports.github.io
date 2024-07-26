---
title: MacPorts 2.10.0 beta2 available
slug: macports-2100-beta2-available
date: 2024-07-26 02:10:30
---

Source code and pkgs for MacPorts 2.10.0-beta2 are now
[available][1]. Testing of either of these install methods is helpful.

Be prepared to encounter bugs. As always, having a recent backup would
be wise. Please [report][2] any bugs that you find (after first [searching
Trac][3], of course!)

There are a large number of changes in this release. See the [ChangeLog][4]
for a list of most of the major ones. You may like to focus your
testing on the new features in that list, as well as your normal usage.

Notable changes since beta1 are:
 * `port migrate` syncs the ports tree before reinstalling ports.
 * Various fixes and improvements to error handling and reporting in the snapshot and restore code.

[1]: https://github.com/macports/macports-base/releases/tag/v2.10.0-beta2
[2]: https://trac.macports.org/newticket
[3]: https://trac.macports.org/search
[4]: https://github.com/macports/macports-base/blob/release-2.10/ChangeLog
