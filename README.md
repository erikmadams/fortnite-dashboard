# KSEL Fortnite Team Analytics Dashboard

A comprehensive web-based analytics dashboard for tracking KSEL (Kern Scholastic Esports League) Fortnite team performance throughout the competitive season.

## Live Dashboard

🔗 **[View Live Dashboard](https://erikmadams.github.io/fortnite-dashboard)**

*Replace `yourusername` with your actual GitHub username*

## Features

### Season Standings
- **Top 30 Teams Display** - Three-column layout showing current rankings
- **Expandable Full Rankings** - View all teams with detailed statistics
- **Playoff Tracking** - Visual indicators for teams that have clinched playoff spots (top 80)
- **Color-Coded Rankings** - Gold, silver, blue, and green badges for different performance tiers

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
- Bakersfield High School
- Bakersfield Christian High School
- Centennial High School
- Central Valley High School
- Cesar Chavez High School
- Del Oro High School
- Delano High School
- East High School
- Foothill High School
- Frontier High School
- Golden Valley High School
- Highland High School
- Independence High School
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
- Vista High School
- Vista West High School
- Wasco High School
- West High School

## Scoring System

The dashboard uses the official KSEL Fortnite scoring system:

### Placement Points
- **1st Place**: 25 points
- **2nd - 5th Place**: 20 points
- **6th - 9th Place**: 15 points
- **10th - 18th Place**: 10 points
- **19th - 25th Place**: 5 points
- **26th+ Place**: 0 points

### Elimination Points
- **4 points per elimination**
- **Maximum 50 points from eliminations**

## Technology Stack

- **Frontend**: HTML5, CSS3 (Tailwind), JavaScript
- **Charts**: Chart.js for performance visualization
- **Icons**: Lucide icons for UI elements
- **Data Source**: Google Sheets integration
- **Hosting**: GitHub Pages

## Setup Instructions

### For Administrators

1. **Clone this repository**
2. **Connect your Google Sheet**:
   - Publish your results sheet as CSV
   - Update the `SHEET_CSV_URL` variable in `index.html`
   - Comment out sample data and uncomment real data functions
3. **Deploy to GitHub Pages**:
   - Enable Pages in repository settings
   - Select source as "Deploy from a branch"
   - Choose `main` branch and `/` (root) folder

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

### For Coaches
- Monitor team performance trends over time
- Compare your team's statistics against other schools
- Track playoff positioning throughout the season
- Analyze game mode performance differences
- Review recent match results and patterns

### For Athletes
- View individual and team achievement metrics
- Track improvement in placement and elimination statistics
- Compare performance against league averages
- Monitor progress toward playoff qualification

## Mobile Compatibility

The dashboard is fully responsive and optimized for mobile devices, allowing athletes and coaches to check statistics on smartphones and tablets between matches.

## Data Updates

The dashboard automatically reflects new data when:
- Match results are submitted through the connected Google Form
- The Google Sheet is updated manually
- Users refresh the dashboard page

*Data typically updates within a few minutes of new entries*

## Support

For technical issues or questions about the dashboard:

1. **Check the Console**: Open browser developer tools (F12) to view any error messages
2. **Verify Data Connection**: Ensure Google Sheet is published and accessible
3. **Clear Browser Cache**: Try a hard refresh (Ctrl+F5 or Cmd+Shift+R)

## Contributing

This dashboard was created for the KSEL Fortnite competitive season. Suggestions for improvements or additional features can be submitted via GitHub issues.

## License

Created for educational use within the Kern Schools Esports League. 

---

**Kern Scholastic Esports League**  
*Tracking Victory Royales and Building Champions*
