# The Software Factory

**[Read it online](https://fss-iot.github.io/software-factory/)**

A lecture deck for a room of IT people who do not program, teaching how software
gets built by agents one station at a time.

**Open `index.html` in a browser.** No server, no internet, no build step.
Pushing to `main` publishes the same page from GitHub Pages.

## Presenting

| Key | Does |
|---|---|
| `→` `↓` `Space` `J` | next station |
| `←` `↑` `K` | previous station |
| `S` | show or hide the speaker notes |
| `F` | full screen |
| `Home` / `End` | first / last slide |

The page scrolls like a document. The keys jump a station at a time, and the bar
at the bottom names where you are. A section taller than the screen scrolls
inside itself before the keys move on.

## The handout

`Ctrl+P` prints one section per page, with the speaker notes included, in
light on white. That is the sheet to hand out at the end.

## What is in it

| # | Section | Min |
|---|---|---|
| 1 | Cover and the promise | 2 |
| 2 | The shift: you run the factory | 4 |
| 3 | The line: seven stations, one loop | 5 |
| 4 | 01 Brief: everything you know, in one dump | 6 |
| 5 | 02 Grilling: the adversarial interview | 10 |
| 6 | 03 Spec: a contract you can test | 6 |
| 7 | 04 Tickets: one behaviour, one check | 7 |
| 8 | 05 Red/green: the check fails first | 8 |
| 9 | 06 Review: a proposal, not a delivery | 6 |
| 10 | 07 Ship: nothing is done until it is live | 5 |
| 11 | Git: commits, branches, pull requests | 8 |
| 12 | Issues and milestones: the plan and the work | 7 |
| 13 | CI/CD: the robot inspector | 8 |
| 14 | The repository remembers the project | 5 |
| 15 | The vault: the agent's memory | 5 |
| 16 | Setup: twenty minutes, once (live) | 15 |
| 17 | What the agent does, what you do | 4 |
| 18 | Five ways factories stall | 5 |
| 19 | Your first lap (exercise) | 10 |
| 20 | Glossary | 2 |
| 21 | Close: the three rules | 3 |

About 2h15 with the live install and the exercise. To cut it to an hour, shorten
the git and CI sections and run the install as a demo instead of hands on.

CI/CD is optional and is the broadest topic here. Teach it after the loop works.
It can run beside the loop, or take over the mechanical half of review (does it
build, do the checks pass, did anything else break). It cannot make the judgment.

Brief, grill and spec are project documents, written once. Tickets through ship
run again on every milestone. The deck says that out loud on the line slide; it is
the thing a room gets wrong if you skip it.

## Editing it

`assets/deck.css` holds all the styling. The colour tokens are copied from the
Tokyo Night Omarchy theme, so you change them in one place.

`index.html` has one `<section class="slide">` per station. The diagrams are
inline SVG, which keeps them sharp on any projector and needs no libraries.
Speaker notes live in `<aside class="notes">` inside each section, and the first
line is the timing.

If you rewrite the story, keep the shape: seven stations, four of them need a
person (brief, spec, review, and the yes that merges), and the loop back to the
brief is what makes it a factory instead of a project.
