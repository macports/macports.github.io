---
title: MacPorts 2.5.0 release candidate 1 available
slug: macports-250-release-candidate-1-available
date: 2018-05-24 11:47:59
---

Source code and pkgs for MacPorts 2.5.0-rc1 are now
[available][1]. Testing of either of these install methods is helpful.

Be prepared to encounter bugs. As always, having a recent backup would
be wise. Please [report][2] any bugs that you find (after first [searching
Trac][3], of course!)

If no show-stopping bugs are found in the next few days, this will
become the 2.5.0 release.

There are a large number of changes in this release. See the [ChangeLog][4]
for a list of most of the major ones. You may like to focus your
testing on the new features in that list, as well as your normal usage.

Changes since beta1 are:

*   Made portindex(1) more robust in the case of more than one port with the
    same name being accidentally added to the tree. (raimue in aa2b75c)

[1]: https://github.com/macports/macports-base/releases/tag/v2.5.0-rc1
[2]: https://trac.macports.org/newticket
[3]: https://trac.macports.org/search
[4]: https://github.com/macports/macports-base/blob/release-2.5/ChangeLog
