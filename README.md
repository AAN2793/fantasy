# Fantasy Tracker

Single-file React fantasy football tracker for Kos's 10-team PPR league.

## Features (v0.1 - rough draft)

- **My Team** — starter lineup, bench, current matchup score
- **Matchups** — all 5 weekly matchups with live scores
- **Standings** — full league standings sorted by record, then points for
- **Players** — searchable, filterable list of all players with YTD + projected stats
- **Watchlist** — star players to track, even if they're not on your roster

## Stack

- Single-file `index.html`
- React 18 via CDN + Babel Standalone
- No build step, no npm install — deploys as static site to Netlify

## Data

Currently using mock data in `index.html`. Swap with Sleeper API once league is created:

- Sleeper docs: https://docs.sleeper.com
- Endpoints needed: `/league/{league_id}`, `/league/{league_id}/rosters`, `/league/{league_id}/users`, `/league/{league_id}/matchups/{week}`, `/stats/nfl/regular/{season}/{week}`

## Deploy

Pushes to `main` auto-deploy to Netlify.
