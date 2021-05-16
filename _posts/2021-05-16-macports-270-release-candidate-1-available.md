---
title: MacPorts 2.7.0 release candidate 1 available
slug: macports-270-release-candidate-1-available
date: 2021-05-16 05:31:01
---

Source code and pkgs for MacPorts 2.7.0-rc1 are now
[available][1]. Testing of either of these install methods is helpful.

Be prepared to encounter bugs. As always, having a recent backup would
be wise. Please [report][2] any bugs that you find (after first [searching
Trac][3], of course!)

If no show-stopping bugs are found in the next few days, this will
become the 2.7.0 release.

There are a large number of changes in this release. See the [ChangeLog][4]
for a list of most of the major ones. You may like to focus your
testing on the new features in that list, as well as your normal usage.

Changes since beta2 are:
 * Fixed build failure on <= 10.6.
 * Adjusted minimum compiler version for C++17.
 * Using `-j1` for the benefit of ninja when `build.jobs` is 1 (instead
   of no `-j` option), and setting `use_parallel_build no` changes the
   value of `build.jobs` to 1 rather than omitting the `-j` option.
 * Checking some more logs for implicit function declarations.
 * Printing some more possibly helpful log locations when configure fails.

[1]: https://github.com/macports/macports-base/releases/tag/v2.7.0-rc1
[2]: https://trac.macports.org/newticket
[3]: https://trac.macports.org/search
[4]: https://github.com/macports/macports-base/blob/release-2.7/ChangeLog
