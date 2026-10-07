# KSEL Fortnite Team Analytics Dashboard

A comprehensive web-based analytics dashboard for tracking Kern Scholastic Esports League (KSEL) Fortnite duo performance throughout the competitive season, from the regular season through the Finals.

## Live Dashboards

**Students and Coaches:**
- **Season Leaderboard**: [KSEL Fortnite Leaderboard](https://erikmadams.github.io/fortnite-dashboard/)

## 2026 Season Format

- **Duos**: each team is two players (P1 and P2)
- **Two game modes**: Battle Royale and Zero Build, each with its own standings. A duo may compete in one or both modes.
- **Regular season**: all matches before the Finals date
- **Finals**: November 7, 2026. Four matches per mode; each duo's best 3 count.

## Features

### Header
- **Last Updated** - Shows the time of the most recent match entry in the sheet
- **Refresh Data** - Reloads the latest results from Google Sheets

### Season Standings
- **Stage Selector** - Switch between Regular Season and Finals standings. The dashboard opens on the Finals view automatically once Finals results exist.
- **Game Mode Selector** - Switch between Battle Royale and Zero Build
- **Top 50 Display** - Five columns of 10 (Top 10, Ranks 11-20, 21-30, 31-40, 41-50). Columns wrap on smaller screens.
- **School Names** - Each duo's school is shown under the team name
- **Expandable Full Rankings** - Show All Teams lists every duo with qualification score, total points, games, wins, top 5 finishes, and eliminations
- **Finals Cutoff Line** - A dashed line in the full rankings marks the last duo in Finals position
- **Color-Coded Rankings** - Gold for 1st place, blue for duos in Finals position, orange for duos that have not yet played enough matches to qualify

### Finals Qualification (Regular Season)
- **Minimum matches**: a duo must play at least 4 matches in a mode to qualify in that mode
- **Qualification score**: average of the duo's best 4 regular-season scores in that mode
- **Finals spots**: the top 50 qualified duos in each mode advance to the Finals
- Duos with fewer than 4 matches are still ranked by their current average, but they do not take a Finals spot
- Matches count separately for each mode. A duo with 3 Battle Royale and 2 Zero Build matches has not yet qualified in either mode.

### Finals Standings
- **Automatic Finals detection** - Any match dated on or after the Finals date (November 7, 2026) is treated as a Finals match. Coaches and students do not need to mark matches as Finals.
- **Finals score** - Total (not averaged) of each duo's best 3 of 4 Finals matches, per mode
- **Mode champions** - The #1 duo in each mode's Finals view wins that mode
- Finals matches never count toward regular-season qualification, so Finals seeding stays fixed on Finals day

### School Cup (Traveling Trophy)
The School Cup rewards the school with the deepest Fortnite program across the regular season and the Finals, not just the school with the single best duo.

**How points are earned:**
- **Regular season** - Each duo in Finals position earns points by its Finals seed in its mode: 1st seed = 50 points, 50th seed = 1 point
- **Finals** - Each duo earns points by its Finals placement (best 3 of 4 matches), worth 1.5x: 1st place = 75 points
- **Depth cap** - Each school's best 5 duos per mode count, for the regular season and for the Finals separately. Most schools have 5 or fewer duos per mode, so all of their qualifying duos count. A school can't win just by entering the most teams.
- **How the cap is set** - The cap equals the league average number of duos competing per school in each mode, rounded to the nearest whole number. A duo has competed in a mode if it submitted at least one result in that mode. For 2026: Battle Royale 86 duos across 17 schools (5.06) and Zero Build 98 duos across 20 schools (4.90), so the cap is 5. It is recalculated once after the roster deadline and then stays fixed for the season.
- **Both modes count** - A duo that qualifies in both Battle Royale and Zero Build can earn points, and Finals berths, in each mode
- **Eligibility** - A school must have at least one duo in the Finals (either mode) to win the trophy
- **Tiebreakers** - More Finals berths first, then the higher-scoring single duo

**Projected tally during the regular season:**
- Until the Finals date, every duo currently ranked in the top 50 of its mode scores by its current rank, even before playing 4 matches. These duos are marked "provisional".
- The Cup panel is labeled "Projected", and schools show "In Finals position" or "Outside top 50"
- On November 7, the Cup switches to official Finals seeds (duos with 4+ matches only), and Finals points are added as results come in

**On the dashboard:**
- **Leader card** - Current Cup leader, point total, and lead over 2nd place
- **Standings table** - Battle Royale season points, Zero Build season points, Finals points, total, Finals berths, and eligibility status. Ineligible schools are grayed out.
- **Point breakdown** - Click any school to see which duos are scoring and how many points each earned. Duos outside a school's best 5 are shown as "not counted".
- **Rules box** - "How School Cup points work" explains the scoring on the page itself

### Filtering & Analysis
- **Filter panel** - Sits directly under Season Standings and the School Cup. Filters apply to every section below it. Season Standings and the School Cup are official standings and are not affected by filters.
- **School Filter** - View performance by individual KSEL schools
- **Team Filter** - Focus on specific duos
- **Game Mode Filter** - Separate Battle Royale and Zero Build statistics

### Team Leaderboards
- **Best Teams** - Ranked by average placement (lower is better)
- **Highest Scoring** - Duos with best average points per game
- **Most Eliminations** - Duos with highest average eliminations

### Player Leaderboards
- **Top Players (Eliminations)** - Total eliminations per player
- **Top Players (Total Damage)** - Total damage dealt per player
- **Top Players (Accuracy)** - Average accuracy per player. Players need accuracy recorded in at least 3 matches to be ranked. Accuracy entered as 0.35, 35, or 35% is all read correctly.
- Players are matched by gamer tag (not case-sensitive), with their team and school shown under the tag

### School Performance
- Schools ranked by average points per match across all of their duos
- Also shows total points, number of duos, matches, wins, top 5 finishes, and eliminations
- Follows the filter panel (for example, filter to Zero Build to rank schools in that mode only)

### Team Performance Analytics
- **Victory Royales** - Win count and win rate percentage
- **Match Statistics** - Total matches played
- **Placement Metrics** - Top 5 and Top 10 finish counts with percentages
- **Elimination Tracking** - Average and total eliminations
- **Performance Trends** - Chart of placement and points over the most recent matches
- **Recent Games** - The 10 most recent matches with school, team, placement, points, and eliminations

## KSEL Schools Supported

The dashboard tracks performance for all participating KSEL schools:

- Arvin High School
- Bakersfield Christian High School
- Bakersfield High School
- Centennial High School
- Cesar Chavez High School
- Del Oro High School
- Delano High School
- East Bakersfield High School
- Foothill High School
- Frontier High School
- Garces Memorial High School
- Golden Valley High School
- Highland High School
- Independence High School
- Kern Valley High School
- Liberty High School
- Mira Monte High School
- North High School
- Ridgeview High School
- Robert F Kennedy High School
- Shafter High School
- South High School
- Stockdale High School
- Tierra Del Sol High School
- Valley High School
- West High School

## Technical Stack

- **Frontend**: HTML5, CSS3 (Tailwind CSS), JavaScript
- **Charts**: Chart.js for data visualizations
- **Icons**: Lucide Icons
- **Data Source**: Google Sheets integration
- **Hosting**: GitHub Pages

### Data Integration

The dashboard connects to your existing Google Sheets data source. Match results entered through your HTML form will automatically appear in the dashboard analytics.

**Sheet Columns Used by the Dashboard**:
- Timestamp
- School
- Team Name
- Date (used to separate regular season from Finals; M/D/YYYY or YYYY-MM-DD)
- Game Mode (Battle Royale or Zero Build)
- Team Placement
- Total Points
- P1 Tag, P1 Elims, P1 Damage, P1 Accuracy
- P2 Tag, P2 Elims, P2 Damage, P2 Accuracy
- Total Eliminations

The sheet also stores assists, revives, damage taken, distance, and hits for each player. The dashboard does not display these yet.

### Configuration Settings

All league rules are settings near the top of the dashboard's script. Change the number and every calculation and on-page label updates to match.

- `QUALIFYING_MATCHES = 4` - Matches needed to qualify, and how many best scores are averaged
- `FINALS_SPOTS = 50` - Finals spots per game mode
- `PREVIEW_RANKS = 50` - Ranks shown in the collapsed Season Standings view
- `FINALS_DATE_STRING = '2026-11-07'` - Matches on or after this date count as Finals
- `FINALS_COUNTING_MATCHES = 3` - Best Finals matches added together for the Finals score
- `CUP_DUOS_PER_MODE = 5` - Duos per school that score in each mode for the School Cup (league average of duos competing per school per mode, rounded)
- `FINALS_CUP_MULTIPLIER = 1.5` - How much Finals points are worth compared to regular-season points
- `MIN_ACCURACY_MATCHES = 3` - Matches with accuracy data needed to appear on the accuracy leaderboard

**Each new season:** update `FINALS_DATE_STRING` to the new Finals date.

## Usage

### Regular Season vs. Finals

**Regular Season** (before the Finals date):
- Standings use the average of each duo's best 4 matches, per mode
- Duos must play at least 4 matches in a mode to qualify
- Top 50 qualified duos per mode advance to the Finals
- The School Cup shows a projected running tally

**Finals** (November 7, 2026):
- Switch Season Standings to the Finals stage (automatic once Finals results exist)
- Standings use the **total of each duo's best 3 of 4 matches**, per mode
- The School Cup locks in official Finals seeds and adds Finals points

### For Coaches
- Monitor team performance trends over time
- Compare your duos' statistics against other schools
- Track Finals positioning in each mode throughout the season
- Follow your school's position in the School Cup race and see which duos are scoring
- Analyze game mode performance differences
- Review recent match results and patterns

### For Athletes
- View individual and team achievement metrics
- See where you rank on the player leaderboards for eliminations, damage, and accuracy
- Track improvement in placement and elimination statistics
- Monitor progress toward Finals qualification
- Follow Finals standings in real time

## Mobile Compatibility

The dashboard is fully responsive and optimized for mobile devices, allowing athletes and coaches to check statistics on smartphones and tablets between matches.

## Data Updates

The dashboard automatically reflects new data when:
- Match results are submitted through the connected results form
- The Google Sheet is updated manually
- Users refresh the dashboard page or click Refresh Data

*Data typically updates within a few minutes of new entries*

## Setup for the Finals

The main dashboard handles the Finals automatically:

1. **Keep all regular-season data in place** - Do not archive or clear the "Match Results" tab. The School Cup needs regular-season and Finals results together.
2. **Confirm the Finals date** - Check that `FINALS_DATE_STRING` matches the Finals day
3. **Enter Finals results as usual** - Use the normal results entry form on Finals day. Make sure the Date field is the Finals date.
4. **View live standings** - Season Standings switches to the Finals view, and the School Cup adds Finals points automatically

**Note:** The separate Grand Championship Standings page reads every row in the "Match Results" tab. Because regular-season data now stays in the sheet, that page will include regular-season matches unless it is updated to use the Finals date. The Finals view on the main dashboard shows the same best-3-of-4 standings.

## Support

For technical issues or questions about the dashboard:

1. **Check the Console**: Open browser developer tools (F12) to view any error messages
2. **Verify Data Connection**: Ensure Google Sheet is published and accessible
3. **Clear Browser Cache**: Try a hard refresh (Ctrl+F5 or Cmd+Shift+R)
4. **Check the Date column**: If a match shows up in the wrong stage (regular season vs. Finals), check the Date entered for that match

For technical support or feature requests, contact the KSEL leadership team.

## Version History

- v3.0 (2026 season): Duos format; best 4 matches (minimum 4) for qualification; top 50 per mode make the Finals; top 50 standings view; Finals stage with automatic Finals-date detection; School Cup traveling trophy standings with projected tally (best 5 duos per mode, based on the league average); player leaderboards (eliminations, damage, accuracy); School Performance table; school names in standings; Last Updated time; filters now apply to all sections below them
- v2.0: Added Grand Championship standings with top 3 of 4 scoring format
- v1.0: Initial release with season analytics dashboard

## License

Developed for Kern Scholastic Esports League by LeagueHQ developers. For KSEL internal use only.
