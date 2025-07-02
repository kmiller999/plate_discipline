# Plate Discipline Dimensionality Reduction

This project analyzed aggregated swing decision data from MLB hitters using Principal Component Analysis (PCA). This model reconstructed the original variance into new components that characterized hitters more efficiently. The two prominent components have notable implications for how plate discipline metrics are discussed and used to characterize hitters.

The rendered [.html version](https://kmiller999.github.io/ds_portfolio/posts/plate_discipline/code/plate_discipline_dr.html) of this project is available on my portfolio website.

## Data Source

The data for these analyses comes from [Baseball Savant's Custom Leaderboard](https://baseballsavant.mlb.com/leaderboard/custom?year=2024&type=batter&filter=&min=q&selections=pa%2Ck_percent%2Cbb_percent%2Cwoba%2Cxwoba%2Csweet_spot_percent%2Cbarrel_batted_rate%2Chard_hit_percent%2Cavg_best_speed%2Cavg_hyper_speed%2Cz_swing_percent%2Coz_swing_percent%2Coz_contact_percent%2Cout_zone_percent%2Cmeatball_swing_percent%2Cmeatball_percent%2Cpitch_count%2Ciz_contact_percent%2Cin_zone_percent%2Cedge_percent%2Cwhiff_percent%2Cswing_percent&chart=false&x=pa&y=pa&r=no&chartType=beeswarm&sort=pa&sortDir=desc) functionality. Qualifying hitters were analyzed for each year from 2021 to 2024. The features used in the PCA model were zone swing %, out of zone swing %, meatball swing %, and overall swing %.

## Data Processing and Modeling

-   PCA was run on scaled metrics for each year separately

-   Intraclass correlation investigated reliability of an individual player's component scores between seasons

## Findings

-   The PCA model reconstructed variance in a way that produced similar constructs between seasons

-   The first two components captured nearly all the variance and represented complementary constructs

-   Hitters varied more in their general tendency to swing than in their tendency to swing at good pitches over bad pitches

-   Hitters' component scores may reflect some variance in how they are pitched, but appeared to have little association to their overall performance

-   Individual hitters' component scores were largely consistent between seasons

## License

This project is licensed under the MIT License (see [LICENSE](LICENSE) for more details).