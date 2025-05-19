# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Repository Overview

This repository contains a simple static website for "Klein Im Hain," which appears to be a kindergarten/childcare center ("Kinderladen" in German). The site consists of a single HTML page with CSS styles and minimal JavaScript.

## Project Structure

- `index.html` - The main (and only) HTML file containing the website structure, inline CSS styles, and a small JavaScript function
- `person1.jpg` and `person2.jpg` - Images used for the team section
- `.github/workflows/static.yml` - GitHub Actions workflow for deploying the static site to GitHub Pages

## Deployment

The site is automatically deployed to GitHub Pages when changes are pushed to the main branch using GitHub Actions as configured in `.github/workflows/static.yml`.

## Development Notes

This is a simple static website without a build process or dependencies. To make changes:

1. Edit the HTML, CSS, or JavaScript in `index.html` directly
2. Test locally by opening `index.html` in a browser
3. Push changes to the main branch to trigger an automatic deployment to GitHub Pages

## Website Structure

The website is divided into several sections:
- Kinderladen (About the kindergarten)
- Team (Staff information)
- Räume (Facilities/rooms)
- Freie Plätze (Available places)
- Praktikum/FSJ (Internship/voluntary social year)
- Verein (About the association)
- Kontakt (Contact information)

The navigation is responsive with a hamburger menu for mobile devices.