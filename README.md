# FIFA World Cup 2026 — Analysis Dashboard

An interactive, single-page analysis dashboard built on publicly available FIFA World Cup 2026 data.

**Live dashboard:** [gitus-maxi-mus.github.io/wc2026-dashboard/](https://gitus-maxi-mus.github.io/wc2026-dashboard/)

---

## What's inside

| Section | Description |
|---|---|
| Tournament Snapshot | Key KPIs — total goals, matches, teams, avg goals per match, highest-scoring game |
| Top Goal Scorers | Top 10 players by goals, 3D horizontal bars |
| Top Contributors | Top 10 players by goals + assists combined, stacked breakdown |
| Team Goal Performance | Diverging bars — goals scored vs goals conceded per team |
| Goals by Confederation | 3D doughnut, goals split across UEFA / CONMEBOL / CONCACAF / CAF / AFC / OFC |
| Goals by Tournament Stage | Animated stat cards per round |
| Venue Performance | Lollipop chart — total goals and matches per venue |
| Goal Timing | 3D vertical bars + polar area — goals by 15-minute interval |
| Shot Conversion Rate | Top 15 teams by goals-per-shot-on-target |
| Disciplinary Records | Stacked yellow + red cards, top 12 teams |
| Player of the Match | Top 10 POTM award winners |
| FIFA Ranking vs Stage | Bubble scatter — pre-tournament ranking vs stage reached, colour-coded by over/underperformance |
| Squad Age Analysis | Avg squad age (all 48 teams) + age range per squad, colour by confederation |
| Player Market Value | Top 15 players + top 20 squads by estimated EUR market value |

## Data sources

All data is sourced from the public dataset by [@mominullptr](https://github.com/mominullptr):

[github.com/mominullptr/FIFA-World-Cup-2026-Dataset](https://github.com/mominullptr/FIFA-World-Cup-2026-Dataset)

Files in `/data`:

| File | Contents |
|---|---|
| `matches_detailed.csv` | Match results, dates, stages, venues, scorelines |
| `match_events.csv` | Goal, card, and substitution events with minute stamps |
| `match_team_stats.csv` | Shots, shots on target, possession per team per match |
| `player_stats.csv` | Goals, assists, and appearances per player |
| `squads_and_players.csv` | Squad composition, DOB, position, club, market value |
| `teams.csv` | Team names, confederation, FIFA ranking |
| `venues.csv` | Stadium names, cities, capacities |

## Tech

- Plain HTML, CSS, JavaScript — no framework, no build step
- [Chart.js 4.4.0](https://www.chartjs.org/) via CDN
- Runs locally from `file://` or via GitHub Pages
- All data embedded as JS constants (no server needed)
