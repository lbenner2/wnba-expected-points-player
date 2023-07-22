# wnba-expected-points-player

This repository calculates the expected point percentage for each WNBA player and how that compares to their team. It also analyzes the player's expected point value further by expected points for and against and compares this to their team to examine the offensive and defensive impact each player has on their team. For instance, if a player has and xPF/40 (expected points for per 40 minutes played) of 73 but the team has an xPF/40 of 75, then the team scores 2 less points when that player is on the floor versus when they're off the floor for each 40 minutes played. This would suggest that this player negatively contributes to the team's offense, however there are two important caveats:
1) xPF/40 takes into account minutes but not pace. So theoretically, if a team has a increased possessions when a player is off the floor, that will make the player seem as if they hinder the offense but really the offense is just faster but not necessarily more efficient without them.
2) This stat does not take into account the other 9 players on the floor which is obviously crucial. With a large sample size this caveat does not seem as significant, but if a player is constantly paired with a bad player it would underestimate their xPF/40.

The first script 'DF_EDITOR_FINAL' calculates each player's efficiency from different spaces on the floor which is crucial for calculated the personal xP values and team xP values.

The second script 'XP_PLAYER_FINAL' iterates through each event in a game and calculates each player and team's xP.

The third script 'xP_PLAYER_MEASUREMENTS_FINAL' summarizes each player and team's xPF and xPA over the season to calculate each player's xPF/40_relative and xPA/40_relative to understand that player's offensive and defensive contributions to a team.

