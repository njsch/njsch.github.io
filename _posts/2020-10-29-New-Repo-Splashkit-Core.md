---
layout: post
title:  "New-ish Forked Project Repository -- splashkit-core"
date:   2020-10-29 14:04:00 +1100
categories: CompSci GitHub Technology Software SDK repo repository.
description: "A new code repository has been added to my GitHub account: splashkit-core.  It basically contains the..."
---

A new code repository was added to my GitHub account: [splashkit-core](https://github.com/njsch/splashkit-core).  It basically contains the core components of an open-source all-purpose [SDK](https://en.wikipedia.org/wiki/Software_development_kit) that Deakin University Computer Science students have been using to write their beginner's-level programs.

Currently I either have added (or am in the process of adding) the following features to [Splashkit](https://www.splashkit.io/):
  - Added [more complete developer documentation](https://github.com/splashkit/splashkit-core/pull/121) for building Splashkit from source on Windows - must immensely thank Deakin's and Swinburn's [Assoc. Prof. Andrew Cain](https://www.deakin.edu.au/about-deakin/people/andrew-cain) for his patience on that one...
  - Added [developer documentation with more detailed instructions](https://github.com/splashkit/splashkit-core/pull/137) on how to write new code and run tests for said code when creating extensions for the Splashkit core SDK itself, so that one no longer has to search through the code or send lots of emails and chats to find the answers.
  - Collaborated with [Hayley Hughes](https://blog.foxes.systems/about/), using the imperatively / structurally-extended procedural programming paradigm to add a [logging module](https://github.com/njsch/splashkit-core/tree/logging) to the core SDK, allowing for third-party applications written with Splashkit to integrate basic logging functionality for info and debugging purposes.  Messages can be written to either a text-based console or a plain text log file.
  - Potential todo: Use Object-orientated Development (OOP) to [add a preferably cross-platform speech and Braille library](https://github.com/splashkit/splashkit-core/issues/113) to enable communication of third-party apps using Splashkit with screen-reader and / or Braille display APIs.  Possibly borrow from [Tolk](https://github.com/dkager/tolk) and / or [Accessible_output2](https://github.com/ctoth/accessible_output2).