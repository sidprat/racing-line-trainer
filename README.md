# Racing Line Trainer

An F1 racing-line trainer: drag a Bezier line through each corner of 20 real
circuits, check it against a computed minimum-lap-time ideal line, and submit
your time to a per-track leaderboard.

Static site, no build step. `index.html` fetches its own source at runtime
(see `support.js`), so it must be served over HTTP — opening it via `file://`
won't work.

React/ReactDOM are vendored locally under `vendor/` (same builds `support.js`
would otherwise pull from unpkg.com) so the app has no third-party CDN
dependency at runtime.
