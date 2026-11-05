---
layout: page
title: "Andrew's Sorting Hat — Interactive Theme Project"
description: "Python speech input, operator-assisted name matching, and sequenced browser video"
category: fun
importance: 2
status: "Software developed; testing and refinement"
related_publications: false
---

## Building an experience for someone else

For Andrew's Harry Potter theme project, I worked on the software behind an interactive Sorting Hat experience. A participant gives their name, the system helps the operator identify them, and the display plays a personalized reveal sequence. It was a chance to apply programming to something playful while dealing with the very practical problem of making it usable on someone else's computer.

## How the interaction works

A **Python application** coordinates microphone input, roster matching, operator choices, and a browser-based video display. Listening begins during the name-prompt video. The software compares the recognized text with the roster and offers up to five candidate matches, leaving the final selection to the operator. Manual entry and a random-house option provide alternatives when recognition is not useful.

The display follows a sequence: **idle → name prompt → thinking clip → house reveal → personal video → house banner → idle**. Keeping the operator controls separate from the audience display lets the operator resolve a name without putting that process on the presentation screen.

## The details that made it an engineering problem

Getting the command flow to run was only part of the work. During troubleshooting, the terminal could be listening and accepting choices while the video window remained blank. I worked through startup ordering, browser autoplay behavior, and media-path handling to make those failures easier to isolate.

The local server also needed **MP4 byte-range support** for browser media requests. I added diagnostics for missing media and playback problems, and checks to prevent a code-only update package from being mistaken for the full application with its video assets.

## Designing for the operator

The Windows launcher opens a movable app-style display that can be switched to fullscreen with F11. The start action can be triggered from the terminal or the display, while the selection controls stay with the operator. Those details came from troubleshooting how the application was actually being launched and used.

The software has been developed and packaged for further testing. This page describes the implementation and debugging work; it does not claim a completed event rollout. The experience reinforced something I enjoy about software engineering: small interface and packaging decisions can determine whether a useful program is usable by someone else.

**Tools and focus:** Python, JavaScript, speech recognition, fuzzy name matching, HTTP media serving, browser playback, and operator workflows.
