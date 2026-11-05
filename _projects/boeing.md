---
layout: page
title: Boeing 777X Flight Controls
description: Flight control verification, simulation, live hydraulic testing, and
  Python engineering tools
importance: 0
category: employment
status: Current role
related_publications: false
permalink: /projects/boeing/
---

**GNC Engineer 2 · Everett, WA · April 2026–Present**

## Working across the Primary Flight Function team

On Boeing's 777X Primary Flight Function (PFF) team, I work across safety analysis, requirements, and testing, with most of my focus on test and verification. I help establish whether flight control behavior meets its requirements through **software-in-the-loop (SIL), hardware-in-the-loop (HIL), and on-aircraft testing**.

The work combines understanding a complex aircraft system with tracing individual signals, building test scenarios, and documenting evidence that supports the Boeing 777-9 certification effort.

## Connecting simulation to physical hardware

I develop aircraft scenario files for the **Psim simulation model** and support their use with the **Integrated Test Vehicle (ITV)**. Connecting the simulated aircraft conditions to live hydraulic hardware lets us evaluate physical system behavior against the conditions created in simulation.

I built a **custom Python parser** to work with scenario files in Python and export simulation and test data to **MATLAB for analysis and report generation**. This work connects software development directly to the engineering test process.

## Making the test workflow easier to use

The scenario files use a syntax closer to C# than Python. I wrote a parser so I could handle that information in Python, then extract data into MATLAB for analysis and report generation. The aim was to make the transition between scenario definition, test output, and documentation easier to manage.

I also noticed that gathering data and writing reports varied across teams. My response was to build a structured template and supporting scripts that give the information a consistent place and prompt the author for the details needed in review. Engineering judgment still sits with the person preparing and reviewing the evidence.

## Finding evidence and resolving discrepancies

I trace upstream and downstream signals in **Simulink** models to identify the evidence needed to verify requirements assigned to test cases. When expected and observed behavior differ, I investigate the discrepancy and support corrections to test cases and documentation.

I also collaborate with engineering stakeholders and the **FAA** in support of certification activities, contributing within the broader PFF safety, requirements, and test process.

## Tools that support the team

- **Structured reporting:** Python tools and reporting templates used by engineering teams across locations to standardize test documentation and guide completion of information needed for Boeing PFF and FAA reviews.
- **Onboarding:** A Python assistant using a local LLM to help PFF contractors find getting-started guidance in the existing team wiki.

## What this work develops

My focus is on connecting the requirement, the model, the physical response, and the resulting test evidence. It draws on systems integration, troubleshooting, software automation, and technical communication.

[View my resume]({{ '/resume/' | relative_url }}) · [Explore my work]({{ '/experience/' | relative_url }})
