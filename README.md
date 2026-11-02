# 🏒 Hockey Stats

A small web app for logging goals from the sideline. It runs from GitHub Pages and you can add it to your phone's home screen like an app. It works offline, and all data is stored on the phone.

- **New match**: enter the opposing team (your own team name is remembered) and press **Create match**. This takes you to the match page. Press **▶ Start match** at face-off, and the date and start time are saved then.
- **Notes**: every match has a notes field for the coach. It saves as you type, and you can edit it before, during or after the match.
- **Live match**: a countdown clock for each period (default 3 × 15 min, set when you start a match), big GOAL buttons for each team, Pause/Resume, End period and Start next period, and End match. The clock stops by itself at 00:00. Each goal records the period, the time played in the period (as on a scoresheet), the time left on the clock, and the total match time.
- **Analysis**: two histograms with one column per minute of P1, P2 and P3. Green shows goals scored and red shows goals conceded, as an average per match. Tap a column to see its numbers. Drag the two handles of the slider at the bottom to include only the matches between them. When you open the page, all matches are included.
- **Export all as CSV**: on a phone this opens the share sheet (save to Files or Drive, send by email, …). On a computer it downloads the file. There is one row per goal, and the match note is in the last column.

## Put it on GitHub Pages

Source: https://github.com/gunnartl/hockeyStats

On GitHub, open the repo and go to **Settings → Pages → Build and deployment**. Choose *Deploy from a branch*, then `main` and `/ (root)`. After a minute the app is live at `https://gunnartl.github.io/hockeyStats/`.

## Add to home screen

- **iPhone (Safari)**: tap the Share button, then **Add to Home Screen**.
- **Android (Chrome)**: tap ⋮, then **Add to Home screen** (or **Install app**).

## Updating

When you change files, bump `VERSION` in `sw.js` so phones fetch the new version. Then close and reopen the app.

⚠️ The data lives only in that phone's browser storage. Export the CSV now and then as a backup. On iPhone, the home-screen app and Safari have **separate** storage, so always use the same one.
