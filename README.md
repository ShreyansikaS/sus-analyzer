# SUS Analyzer

A tool for scoring System Usability Scale (SUS) surveys, which is a standard 10 question questionnaire used in usability research.

Live demo: https://YOUR-USERNAME.github.io/sus-analyzer/

## Why I made this
My research work is mostly about how people behave in experiments, and a lot of that is cleaning survey data and making sure the scoring is right. SUS has a scoring rule that is easy to get wrong because odd and even questions are scored in opposite directions. I built this to practice turning a research method into a tool that other people could use without a spreadsheet.

## What it does
Paste responses (one participant per line, ten numbers from 1 to 5) or upload a CSV. It gives each participant a score out of 100, the average, standard deviation, minimum and maximum, and a rough grade. If the data has a mistake, like a missing answer or a 7, it tells you which row is wrong. You can download the results as a CSV.

## What I did
- Implemented the SUS scoring rule: odd items count as response minus 1, even items count as 5 minus response, and the total is multiplied by 2.5.
- Added input validation with row level error messages.
- Added a warning when the sample is small, since an average from three people does not mean much.
- Built CSV import and export.

## Skills used
UX research methods, survey scoring, descriptive statistics, JavaScript, data validation, file handling in the browser, HTML, CSS.

## Roles this project fits
UX Researcher, Quantitative UX Researcher, Research Assistant, Data Analyst, UX Engineer (research tools).

## Run it
Open `index.html` in a browser. Sample data is already filled in so you can click Calculate right away.

## What I would add next
Confidence intervals, and a way to compare two versions of a design with a t-test.
