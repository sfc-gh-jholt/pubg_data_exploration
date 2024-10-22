# PUBG Data Analysis

## About the Dataset

This dataset contains anonymized statistics from PlayerUnknown's Battlegrounds (PUBG) matches. In each match, up to 100 players participate and can be on teams that get ranked at the end of the game based on survival. Players can pick up items, engage in combat, revive teammates, and traverse the map in various ways. The data includes a wide variety of in-game activities and player stats, including those related to combat, movement, and team dynamics.

Each row in the dataset represents the post-game stats of an individual player from matches of all types: solo, duo, squad, and custom games. It is important to note that there is no guarantee of exactly 100 players per match or at most 4 players per group.

## File Description

- **`data.csv`**: This is a 151MB CSV file containing the post-game statistics for PUBG players.

## Data Fields

The following fields are included in the dataset:

- **DBNOs**: Number of enemy players knocked.
- **assists**: Number of enemy players damaged by this player and killed by teammates.
- **boosts**: Number of boost items used.
- **damageDealt**: Total damage dealt (self-inflicted damage is subtracted).
- **headshotKills**: Number of enemy players killed with headshots.
- **heals**: Number of healing items used.
- **Id**: Player's unique identifier.
- **killPlace**: Ranking based on the number of enemy players killed.
- **killPoints**: Kills-based external ranking of players (akin to an Elo rating for kills).
- **killStreaks**: Maximum number of kills in a short time.
- **kills**: Total number of enemy players killed.
- **longestKill**: Longest distance between the player and the killed enemy at the time of death.
- **matchDuration**: Duration of the match in seconds.
- **matchId**: Unique identifier for each match.
- **matchType**: Game mode (e.g., "solo", "duo", "squad", "solo-fpp", etc.).
- **rankPoints**: Elo-like ranking of players. Value of -1 indicates "None".
- **revives**: Number of times the player revived teammates.
- **rideDistance**: Total distance traveled in vehicles (in meters).
- **roadKills**: Number of kills while in a vehicle.
- **swimDistance**: Total distance traveled by swimming (in meters).
- **teamKills**: Number of times the player killed a teammate.
- **vehicleDestroys**: Number of vehicles destroyed.
- **walkDistance**: Total distance traveled on foot (in meters).
- **weaponsAcquired**: Number of weapons picked up.
- **winPoints**: Win-based external ranking of players (akin to an Elo rating for winning).
- **groupId**: Unique identifier for each group within a match.
- **numGroups**: Number of groups in the match.
- **maxPlace**: Worst placement available in the match.
- **winPlacePerc**: The percentile winning placement for the player (target for prediction). It is based on `maxPlace` and ranges from 0 to 1, where 1 is 1st place and 0 is last place.

## Usage

This dataset can be used for a variety of purposes, including:

- **Predictive Modeling**: Predict the `winPlacePerc` for each player using other features in the dataset.
- **Exploratory Analysis**: Understand player behavior, team dynamics, and factors contributing to in-game success.
- **Feature Engineering**: Create meaningful features to enhance predictive performance (e.g., kill-to-distance ratios, healing rate, etc.).

The dataset is formatted for machine learning tasks, such as training models to predict winning percentages or analyzing player strategies.

## Getting Started

To use the dataset, you can load it into your data analysis tools (e.g., Python with Pandas, R, etc.). Here are a few suggested starting points:

1. **Visualize** the distribution of key metrics like kills, damage dealt, and distances traveled.
2. **Analyze** the correlation between different features and the winning percentile (`winPlacePerc`).
3. **Develop** models that predict player performance based on in-game stats.

Happy analyzing, and good luck with your battle for Chicken Dinner!

## License

This project is licensed under the [MIT License](LICENSE).

## Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

## Acknowledgments

- **PUBG Corporation** for providing the dataset.
- **Kaggle** for hosting the dataset and providing the platform for analysis.

## Contact

For questions or suggestions, please create an issue or contact the project maintainers.
