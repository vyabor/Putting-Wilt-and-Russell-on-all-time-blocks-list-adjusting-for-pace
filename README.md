# Putting-Wilt-and-Russell-on-all-time-blocks-list-adjusting-for-pace
Using data from stats.nba.com as well as user gathered data on blocked shots per game of Wilt Chamberlain and Bill Russell found at https://www.reddit.com/r/nba/comments/3s9669/heres_135_nba_games_where_blocked_shot_data/ , the following is a function to append the all time leaderboard in blocks per game to have Wilt Chamberlain and Bill Russell adjusted for pace.

From the data found on reddit, Wilt Chamberlain averaged 8.8 blocks per game (651 blocks in 74 games) in the regular season as well as 8.3 blocks per game (316 blocks in 38 games) in the playoffs.
According to the sample data, Bill Russell averaged 8.6 blocks per game (704 blocks in 85 seasons) in the regular season as well as 7.7 blocks per game (384 blocks in 50 games) in the playoffs.

In order to adjust stats for Pace, one would multiply the stat by the ratio of the current season's pace to that of the era which you are comparing. For example, the average pace over Wilt's career was 119.16. To adjust his regular season blocks average, I did 8.8*(100.2/119.16) = 7.37 blocks per game.

I've written something short and simple in Python that first adjusts their blocks per game stats for pace to the current era and concats the all time leaders list in blocks per game with their newly adjusted stats.
