---
title: MacPorts 2.11.0 release candidate 1 available
slug: macports-2110-release-candidate-1-available
date: 2025-06-27 17:30:00
---

Source code and pkgs for MacPorts 2.11.0-rc1 are now
[available][1]. Testing of either of these install methods is helpful.

Be prepared to encounter bugs. As always, having a recent backup would
be wise. Please [report][2] any bugs that you find (after first [searching
Trac][3], of course!)

If no show-stopping bugs are found in the next few days, this will
become the 2.11.0 release.

There are a large number of changes in this release. See the [ChangeLog][4]
for a list of most of the major ones. You may like to focus your
testing on the new features in that list, as well as your normal usage.

Changes since beta1 are:
 * Fixed possible permissions error when syncing. (#72624)
 * Made 'port snapshot' with no options behave as documented. (#72628)
 * Fixed error getting the default developer_dir value when neither
     Xcode nor the Command Line Tools are installed. (#72644)
 * Added some missing documentation for new features. (#72627)

[1]: https://github.com/macports/macports-base/releases/tag/v2.11.0-rc1
[2]: https://trac.macports.org/newticket
[3]: https://trac.macports.org/search
[4]: https://github.com/macports/macports-base/blob/release-2.11/ChangeLog
