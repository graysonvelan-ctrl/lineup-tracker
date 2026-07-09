# Lineup +/- & Rating Tracker

A browser-based tool for tracking basketball player and lineup performance during games and calculating offensive / defensive / net net ratings.

**Live app:** https://graysonvelan-ctrl.github.io/lineup-tracker/

## What it does

As a game is tracked, the you can use the app to record points and possessions for both teams along with which five players are on the court at any given time. From that data it calculates:

- Plus/minus
- Offensive rating (points scored per 100 offensive possessions)
- Defensive rating (points allowed per 100 defensive possessions)
- Net rating (offensive rating minus defensive rating)
- Offensive and defensive possessions played

for every individual player and every five-man lineup on both teams

The results are shown as tables and can be exported to CSV.

## How it works

The user first enters both teams' rosters and starting fives. During the game, each team's points and possessions are logged with a tap, and substitutions update which players are on the court. Because a possession for one team is by definition a defensive possession for the other, logging one offensive possession credits both sides automatically.

Every stat is attributed to the players and lineup on the court at the moment it occurs, which is what allows the per-player and per-lineup ratings to be broken out. The data can be generated at any point during the game, not just at the end.

Games are saved in the browser as they are tracked, so closing or refreshing the page does not lose progress.

## Built with

Vanilla HTML, CSS, and JavaScript in a single self-contained file. It runs entirely in the browser with no server or dependencies, and works offline.
