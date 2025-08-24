# CSV files column guide
This document explains the meaning of each column.


## Batting.csv


### Columns

- **Player ID**  
  A unique numerical identifier for each player in Cricinfo’s database. Used internally to track a player.

- **Name**  
  The player’s name.

- **Year**  
  The year (or season) when the stats were recorded.

- **RUNS**  
  Total runs scored by the player in that year/season.

- **Six**  
  Number of sixes hit (shots clearing the boundary without bouncing).

- **Four**  
  Number of fours hit (shots crossing the boundary after bouncing).

- **BF (Balls Faced)**  
  The number of deliveries the player faced.

- **Min (Minutes Batted)**  
  Time spent batting, in minutes. This is more common in Test/longer format stats.

- **Pos (Position)**  
  The batting position (e.g., 1 = opener, 4 = No. 4 batsman).

- **Average of SR (Strike Rate)**  
  Average of strike rates across matches/innings.  
  Strike Rate (SR) = **(Runs / Balls Faced) × 100**.  
  "Average of SR" means they’ve averaged the strike rate per match or per innings across the season.

- **Match Count**  
  The number of matches included in the dataset for that year/season.

- **season_yr**  
    The season year tag (for example, in IPL you may see "2016", "2017"; in domestic tournaments it marks the season year).

---

### Example

If **Virat Kohli** in **2016 IPL** has:  
- Runs: 973  
- Six: 38  
- Four: 83  
- BF: 640  
- Pos: 3  
- Avg SR: 152.0  
- Match Count: 16  
- season_yr: 2016  

That means he scored 973 runs in that season at position 3, facing 640 balls, with a strike rate (on average) of about 152.

---

### Note on Strike Rate

There are two ways strike rate can be reported:

- **Overall SR** = (Total Runs / Total Balls) × 100  
- **Average of SR** = Mean of strike rates from each match/innings  

### Player CSV

- **ID**
Unique identifier for the player in Cricinfo’s database.

- **Name**
Short/common name of the player (e.g., Virat Kohli).

- **Role**
General role category of the player: Batsman, Bowler, Allrounder, Wicketkeeper.

- **Full Name**
The player’s full official name.

- **DOB (Date of Birth)**
Player’s birth date (used to calculate age).

- **Batting Style (s)**
Short form of batting style, e.g., RHB (Right-Hand Bat), LHB (Left-Hand Bat).

- **Bowling Style (s)**
Short form of bowling style, e.g., RM (Right-arm Medium), LB (Leg Break).

- **Batting Style (l)**
Long form of batting style, e.g., Right-hand bat, Left-hand bat.

- **Bowling Style (l)**
Long form of bowling style, e.g., Right-arm medium-fast, Slow left-arm orthodox.

- **Playing Role**
Specific role within the team: Top-order Batter, Middle-order Batter, Opening Bowler, Wicketkeeper Batter, Allrounder.


### Bowling CSV

- **Player ID**
    Unique identifier for the player in Cricinfo’s database.

- **Name**
    Player’s name.

- **Year**
    The season/year when the stats were recorded.

- **Over**
    Number of overs bowled (1 over = 6 legal deliveries).

- **BPO (Balls Per Over)**
    Number of balls bowled per over. Normally 6, but in older cricket (pre-1980s, some countries used 4, 5, 8-ball overs).

- **Mdns (Maidens)**
    Count of maiden overs (overs where no runs were conceded).

- **Runs**
    Runs conceded while bowling.

- **Wkts (Wickets)**
    Total wickets taken by the player.

- **Average of Econ (Economy Rate)**
    Average economy rate across matches/innings.
    - Economy Rate = Runs Conceded ÷ Overs Bowled

    “Average of Econ” means the economy was averaged per match 
    *or innings, not just one calculation on totals.

- **Sum of Pos (Bowling Position)**
    Sum of bowling positions across matches. Bowling position usually refers to the order in which the bowler bowled (e.g., opening bowler = 1, second-change = 5, etc.). Summed across all games.

- **Count of match_id**
    The number of matches included in the dataset for that year/season.

- **season_yr**
    Season year tag (e.g., “2016”, “2017”).