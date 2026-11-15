# The Software Factory

**[Read it online](https://fss-iot.github.io/software-factory/)**

The seed it teaches: **[FSS-IoT/software-factory-vault](https://github.com/FSS-IoT/software-factory-vault)**

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
| hover top-left, or click `☰` | contents, any section in one click |

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
| 3 | Setup: twenty minutes, once (live) | 15 |
| 4 | The vault: the agent's memory | 5 |
| 5 | The line: four stations, one loop | 5 |
| 6 | Before the loop: the brief, one sentence | 6 |
| 7 | Before the loop: the adversarial interview | 10 |
| 8 | Before the loop: a spec you can test | 6 |
| 9 | 01 Tickets: one behaviour, one check | 7 |
| 10 | 02 Red/green: the check fails first | 8 |
| 11 | 03 Review: a proposal, not a delivery | 6 |
| 12 | 04 Ship: closes the milestone | 5 |
| 13 | Git: commits, branches, pull requests | 8 |
| 14 | Issues and milestones: the plan and the work | 7 |
| 15 | CI/CD: the robot inspector (optional) | 8 |
| 16 | The repository remembers the project | 5 |
| 17 | What the agent does, what you do | 4 |
| 18 | Five ways factories stall | 5 |
| 19 | Your first lap (exercise) | 10 |
| 20 | Glossary | 2 |
| 21 | Close: the three rules | 3 |

About 2h15 with the live install and the exercise. To cut it to under two hours,
run the install as a demo instead of hands on, and shorten the git and CI
sections.

CI/CD is optional and is the broadest topic here. Teach it after the loop works.
It can run beside the loop, or take over the mechanical half of review (does it
build, do the checks pass, did anything else break). It cannot make the judgment.

Brief, research, grill and spec come before the loop and happen once per project.
The four stations then run again on every milestone. The deck says that out loud on
the line slide; it is the thing a room gets wrong if you skip it.

## Editing it

`assets/deck.css` holds all the styling. The colour tokens are copied from the
Tokyo Night Omarchy theme, so you change them in one place.

`index.html` has one `<section class="slide">` per station. The diagrams are
inline SVG, which keeps them sharp on any projector and needs no libraries.
Speaker notes live in `<aside class="notes">` inside each section, and the first
line is the timing.

If you rewrite the story, keep the shape: four stations in the loop, a plan before
them that is not a station, and a ship that closes the milestone. The person is
needed at the plan and at the review.
