# Sangha community lists, statistics: the password-protected page

**The page: https://yoboss283.github.io/sangha-community-stats/**
Open the link and enter the password. Ask the owner for the password, and please don't share it outside the community.

## What this repository is

This repository is only the **shop window**: it holds the finished report page, `index.html`, locked with a password.
That is why the file looks like unreadable text: it is encrypted on purpose. Without the password nothing in it can be read.
It has to be a public repository because the free GitHub Pages service only publishes public repositories.

## Where the readable source is

The working project is a separate **private** repository, `yoBoss283/sangha-statistics`. It has the normal source code, the
data, the rules (METHOD.md), the update instructions (UPDATE.md) and the full README. Anyone the owner invites as a
collaborator can read all of it there (GitHub: the repository's Settings, then Collaborators).

## What the report shows

Statistics from the Sangha community lists, 1996 to now, using the Vassa lists as the yearly count and the Winter lists as a
reference:
- the size of the community, the new crop (anagārikas and sāmaṇeras), the monasteries on the list;
- seniority, who comes and goes, how long monks stay, who moves between monasteries;
- nationalities, Pāli names given again, long-term lay residents;
- a lookup: type a name and see every list that person is on, where they stayed, and the years at each place.

It is a small, light exercise to show how the community has changed. The lists can't tell everything, and it doesn't
try to be complete or exactly accurate.

## Updating this page (for the owner and their AI)

The report is rebuilt in the private repository. Then `node encrypt_page.js sangha-statistics.html index.html` locks it
(the password is given as `PAGE_PASSWORD` for that one command and is never saved), and the new `index.html` is pushed here.
The details are in the private repository's `CLAUDE.md` and `UPDATE.md`.
