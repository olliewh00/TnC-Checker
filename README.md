# Terms & Conditions Simplifier

A simple, multi-page web app that helps users quickly understand potential privacy risks in Terms & Conditions text.

## Overview

Most people accept Terms & Conditions without reading them fully. This project provides a plain-language summary and a privacy risk score using client-side keyword detection.

- No frameworks
- No backend
- No API calls
- Built with HTML, CSS, and vanilla JavaScript only

## Features

- Large textarea for pasting Terms & Conditions text
- Simplify button to run analysis
- Output section with:
  - Simplified summary in bullet points
  - Privacy warning bullet points
  - Privacy score (Low Risk, Medium Risk, High Risk)
- No-risk message when no keywords are detected
- Typewriter intro text effect on the home page
- Multi-page site with working navigation

## Scoring System

Keyword points:

- third party -> +2
- location -> +2
- tracking -> +2
- cookies -> +1
- personal information -> +1

Risk tiers:

- 0-2: Low Risk
- 3-4: Medium Risk
- 5+: High Risk

## Keyword Detection

The app scans for these terms:

- third party
- data sharing
- location
- cookies
- tracking
- personal information

When matched, the app shows user-friendly warnings, for example:

- Your data may be shared with third parties.
- This service may track your location.
- Cookies are used to monitor your behavior.

## Project Structure

- index.html: Home page + simplifier tool
- how-it-works.html: Explanation of the analysis flow
- why-this-matters.html: Why policy transparency matters
- privacy-first-analysis.html: Privacy model and data handling details

## How To Run

This is a static site. You can run it in either of these ways:

1. Open index.html directly in your browser.
2. Or serve the folder with a simple local server.

Example using Python:

```bash
python3 -m http.server 8000
```

Then open:

- http://localhost:8000/

## Notes

- Analysis is keyword-based, not legal advice.
- Results are quick indicators to help users review policies more carefully.
- All analysis runs in the browser session.

## License

Use and modify freely for learning and portfolio use.
