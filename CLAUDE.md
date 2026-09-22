# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project status

This repository is at an early stage: it currently contains only `README.md`. There is no source code, build system, dependency manifest, linter config, or test suite yet, so there are no build/lint/test commands to document. Update this file once code is added.

## Project overview (from README)

CS370 (Operating Systems, Colorado State University) term project: "The Plant Owner's Capable Assistant" — a mini houseplant assistant that measures **soil moisture** and **light exposure** so a user can give their plants better care.

Course constraints stated in the README:
- Must address a real-world problem with a solution that isn't easily handled by a plain app.
- Must run on a low-cost single-board computer (Raspberry Pi) with a **minimum of two sensors** (soil moisture and light are the planned pair).

## Working in this repo

- Development happens under WSL2 on a Windows-mounted path (`/mnt/c/...`); hardware-specific code (GPIO/sensor access) can only be exercised on the Raspberry Pi itself, so keep sensor I/O separable from logic that can be tested on a dev machine once code exists.
- Default branch is `main`.
