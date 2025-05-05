# AFC World Cup Qualifiers 2026 Shot Map Visualization

A comprehensive visualization tool for analyzing shot patterns, goal efficiency, and performance metrics of top scorers in the AFC World Cup Qualifiers 2026.

## Overview

This project creates detailed shot map visualizations for the top 9 goal-scorers in the AFC World Cup Qualifiers 2026. Each visualization includes shot distribution, goal locations, and key performance metrics, allowing for in-depth analysis of player efficiency and shooting patterns.

## Features

- **Shot Distribution Heatmaps**: Blue intensity shows concentration of shots in different areas
- **Goal Placement**: Red dots indicate goals (excluding penalties)
- **Performance Metrics**: Comprehensive statistics including np Goals per 90, xG, shooting accuracy
- **Average Shot Distance**: Visual indicator of typical shooting range
- **Shot Placement Accuracy (SPA)**: Semi-circular gauge showing accuracy percentage
- **Team Representation**: Team logos and colors for quick visual identification
- **Customizable Layouts**: 3x3 grid layout with individual player cards

## Data Included

The visualization includes the following key data points for each player:

- **Base Info**: Name, team, position, age, games played, minutes (in 90s)
- **Goal Stats**: Total goals, non-penalty goals, penalties
- **Shot Stats**: Total shots, shots on target, shot accuracy
- **Efficiency Metrics**: Goals per shot, goals per shots on target, xG values
- **Position Data**: Shot coordinates, goal locations, average shot distance

## Top Featured Players

1. ALMOEZ ALI (Qatar) - 12 goals
2. SON HEUNG-MIN (South Korea) - 10 goals
3. MEHDI TAREMI (Iran) - 9 goals
4. SARDAR AZMOUN (Iran) - 8 goals
5. AYMEN HUSSEIN (Iraq) - 7 goals
6. FÁBIO LIMA (UAE) - 8 goals
7. YAZAN AL-NAIMAT (Jordan) - 8 goals
8. AYASE UEDA (Japan) - 8 goals
9. MUSA AL-TAAMARI (Jordan) - 7 goals

## Installation Requirements

```bash
pip install pandas numpy matplotlib mplsoccer pillow
```

## Directory Structure

```
project/
│
├── afc_shot_map.py        # Main visualization script
├── afc_shot_map.png       # Output visualization
├── create_afc_logos.py    # Helper script to generate team logos
│
├── logo/                  # Team logo directory
│   ├── qatar.png
│   ├── korea.png
│   ├── iran.png
│   └── ...
│
└── data/                  # Optional data directory
    └── afc_players.csv    # Player data in CSV format
```

## Usage

1. **Basic Usage**:
```bash
python afc_shot_map.py
```

2. **Generate Team Logos** (if needed):
```bash
python create_afc_logos.py
```

3. **Custom Output Path**:
```bash
python afc_shot_map.py --output custom_output.png
```

## Understanding the Visualization

Each player card in the visualization contains:

- **Player Name and Info**: Team, position, games played, minutes in 90s
- **Shot Statistics**: Total shots, npxG (non-penalty expected goals), npG (non-penalty goals)
- **Shot Map**: Blue heatmap showing shot concentration, white dots for all shots, red dots for goals
- **Performance Metrics**:
  - npG: Non-penalty goals per 90 minutes
  - npxG: Non-penalty expected goals per 90 minutes
  - S: Shots per 90 minutes
  - SoT%: Shot on target percentage
  - npxG/S: Non-penalty expected goals per shot
- **Average Shot Distance**: Shown with red text and arrow (e.g., "12.4 meters")
- **SPA Indicator**: Semi-circle gauge showing Shot Placement Accuracy

## Extending the Visualization

You can extend the visualization by:

1. Adding more players
2. Customizing the metrics displayed
3. Creating alternative layouts (single player, comparative views)
4. Adding temporal analysis (performance over time)
5. Integrating with live data sources

## Credits

- Player data sourced from official AFC statistics
- Shot map methodology adapted from soccer analytics best practices
- Team logos generated based on official team colors

## License

This project is licensed for personal and educational use. All data related to the AFC World Cup Qualifiers belongs to their respective owners.

## Contact

For questions, improvements, or collaboration, please reach out to [me].

---

*Last updated: May 2025*
