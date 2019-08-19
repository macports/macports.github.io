---
title: New ports database site
slug: new-ports-database-site
date: 2019-08-19 03:35:17
---

MacPorts' new ports database is live at [ports.macports.org][1]. Please
consider installing the "mpstats" port to enable submission of
anonymous information about your system and installed ports for
statistical purposes.

The information collected is currently:
* MacPorts version
* OS name and version
* CPU architecture
* Selected C++ standard library
* Xcode, command line tools, and GCC versions
* Name, version, selected variants, and requested status of each installed port
* A UUID so we can tell whether submissions are from distinct users

The site also shows which OS versions each port was successfully built
on, has links to open Trac tickets, and more.

This new site is the result of much hard work by our GSoC student,
Arjun Salyan. We hope you find it useful.

[1]: <https://ports.macports.org/>
