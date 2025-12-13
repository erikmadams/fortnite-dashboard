# KSEL Fortnite Team Analytics Dashboard

A comprehensive web-based analytics dashboard for tracking Kern Scholastic Esports League (KSEL) Fortnite team performance throughout the competitive season.

## Live Dashboards

**Students and Coaches:**
- **Season Leaderboard**: [KSEL Fortnite Leaderboard](https://erikmadams.github.io/fortnite-dashboard/)
- **Grand Championship Standings**: [KSEL Grand Championship](https://erikmadams.github.io/fortnite-dashboard/grand-championship-standings.html)

## Features

### Season Standings
- **Top 30 Teams Display** - Three-column layout showing current rankings
- **Expandable Full Rankings** - View all teams with detailed statistics
- **Playoff Tracking** - Visual indicators for teams that have clinched playoff spots
- **Color-Coded Rankings** - Gold, silver, blue, and green badges for different performance tiers

### Grand Championship Standings
- **Championship Format** - Displays top 3 out of 4 match scores (total, not averaged)
- **Game Mode Filtering** - Toggle between Battle Royale and Zero Build results
- **Real-Time Rankings** - Live standings updated from match results
- **Streamlined View** - Focused display for championship tournament tracking
- **Top 30 Quick View** - Expandable to show all competing teams

### Team Performance Analytics
- **Victory Royales** - Win count and win rate percentage
- **Match Statistics** - Total matches played
- **Placement Metrics** - Top 5 and Top 10 finish counts with percentages
- **Elimination Tracking** - Average and total eliminations

### Interactive Leaderboards
- **Best Teams** - Ranked by average placement (lower is better)
- **Highest Scoring** - Teams with best average points per game
- **Most Eliminations** - Teams with highest average eliminations

### Filtering & Analysis
- **School Filter** - View performance by individual KSEL schools
- **Team Filter** - Focus on specific teams
- **Game Mode Filter** - Separate Battle Royale and Zero Build statistics
- **Performance Trends** - Visual charts showing performance over time
- **Recent Games** - Detailed match history with results

## KSEL Schools Supported

The dashboard tracks performance for all participating KSEL schools:

- Arvin High School
- Bakersfield Christian High School
- Bakersfield High School
- Centennial High School
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
- McFarland High School
- Mira Monte High School
- North High School
- Ridgeview High School
- Shafter High School
- South High School
- Stockdale High School
- Taft High School
- Tehachapi High School
- Valley Home Education Academy
- Wasco High School
- West High School

## Technical Stack

- **Frontend**: HTML5, CSS3 (Tailwind CSS), JavaScript
- **Charts**: Chart.js for data visualizations
- **Icons**: Lucide Icons
- **Data Source**: Google Sheets integration
- **Hosting**: GitHub Pages

### Data Integration

The dashboard connects to your existing Google Sheets data source. Match results entered through your HTML form will automatically appear in the dashboard analytics.

**Required Sheet Columns**:
- Timestamp
- School
- Team Name
- Date
- Game Mode
- Team Placement
- Total Points
- Player statistics (eliminations, damage, etc.)
- Total Eliminations

## Usage

### Season Dashboard vs. Grand Championship

**Season Dashboard** (`index.html`):
- Tracks performance across the entire regular season
- Uses average of top 5 scores out of all matches played
- Shows comprehensive team statistics and trends
- Includes playoff qualification tracking

**Grand Championship** (`grand-championship-standings.html`):
- Specifically designed for championship tournament format
- Calculates standings using **top 3 out of 4 match scores**
- Reports **total points** (not averaged) from best 3 matches
- Streamlined interface focused on live tournament standings
- Each game mode (Battle Royale / Zero Build) tracked separately

### For Coaches
- Monitor team performance trends over time
- Compare your team's statistics against other schools
- Track playoff positioning throughout the season
- Analyze game mode performance differences
- Review recent match results and patterns
- View championship standings during finals

### For Athletes
- View individual and team achievement metrics
- Track improvement in placement and elimination statistics
- Compare performance against league averages
- Monitor progress toward playoff qualification
- Follow championship tournament progress in real-time

## Mobile Compatibility

The dashboard is fully responsive and optimized for mobile devices, allowing athletes and coaches to check statistics on smartphones and tablets between matches.

## Data Updates

The dashboard automatically reflects new data when:
- Match results are submitted through the connected Google Form
- The Google Sheet is updated manually
- Users refresh the dashboard page

*Data typically updates within a few minutes of new entries*

## Setup for Grand Championship

When preparing for the Grand Championship tournament:

1. **Archive Season Data**: Move all regular season data from the "Match Results" tab to a separate tab (e.g., "2025 FN Season Results")
2. **Clear Match Results Tab**: Keep the tab name as "Match Results" but remove all data rows (keep headers)
3. **Run 4 Championship Matches**: Enter results for all 4 championship matches using your normal results entry system
4. **View Live Standings**: The Grand Championship page will automatically calculate and display top 3 out of 4 scores

## Support

For technical issues or questions about the dashboard:

1. **Check the Console**: Open browser developer tools (F12) to view any error messages
2. **Verify Data Connection**: Ensure Google Sheet is published and accessible
3. **Clear Browser Cache**: Try a hard refresh (Ctrl+F5 or Cmd+Shift+R)

For technical support or feature requests, contact the KSEL leadership team.

## Version History

- v2.0: Added Grand Championship standings with top 3 of 4 scoring format
- v1.0: Initial release with season analytics dashboard

## License

Developed for Kern Scholastic Esports League by LeagueHQ developers. For KSEL internal use only.
