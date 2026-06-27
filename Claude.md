# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

# Reading Tracker — Project Briefing

## What this project is
A personal reading tracker. Users can add books to a library, set a reading status, and assign a star rating. Built as a static web app for personal use, deployed to GitHub Pages.

## Tech stack
- HTML, CSS, JavaScript (no frameworks)
- localStorage for data persistence
- Plain CSS only — no CSS frameworks or external libraries

## Running the app
Open `index.html` directly in a browser, or serve it with any static file server (e.g. `python3 -m http.server`). There is no build step, no bundler, and no package manager.

## Decisions already made — do not revisit these
- Data is stored in localStorage — do not change this
- The add button stays greyed out until title, author, and page count are all filled
- Duplicate entries are blocked — same title and same author, case-insensitive
- Rating (0–5 stars, including half stars) is only available for books with "read" status
- This is a static site — no server-side logic, no database, no backend

## Working preferences
- Do not make assumptions — if something is unclear, ask before proceeding
- Use plan mode before starting any build — propose what you're going to do and wait for approval before writing any code
- Pause before adding any feature not explicitly listed in the session spec
- Do not modify any file not directly related to the current task
- Make one change at a time
- Verify all must-haves from the session spec against actual behaviour before considering the session done
