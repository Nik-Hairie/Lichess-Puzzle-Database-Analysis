<h1>Data Analysis: Lichess Puzzle Database</h1>

<h2>Introduction</h2>
This is an analysis on Lichess Puzzle Database obtained from https://database.lichess.org/#puzzles. The database has over 3,080,529 chess puzzles to be analyzed. The puzzles database consists of fields as follows: PuzzleId, FEN, Moves, Rating, RatingDeviation, Popularity, NbPlays, Themes, GameUrl, OpeningFamily, OpeningVariation. Fields that were set aside includes PuzzleId, FEN, Moves, RatingDeviation, GameUrl, Opening Family and OpeningVariation. Data cleaning was performed on Rating, Popularity, NbPlays and Themes because it is relevant for the data analysis.

<h2>Abbreviations</h2>

- Puzzle Rating Range: (545 to 3024)

`<1200: Puzzles rating below 1200`

`<1800: Puzzles rating between 1200 and 1800`

`<2200: Puzzles rating between 1800 and 2200`

`>=2200: Puzzles rating more than 2200`

- Puzzle Popularity Range: (-100 to 100)

`1 - Unpopular: Puzzles popularity below -60`

`2 - Disliked: Puzzles popularity between -60 and -20`

`3 - Mediate: Puzzles popularity between -20 and 20`

`4 - Liked: Puzzles popularity between 20 and 60`

`5 - Popular: Puzzles popularity between 60 and 100`

- NbPlays Range: (0 to 310341)

`<51,725 plays: Puzzles with less than 51,725 number of plays`

`<103,450 plays: Puzzles between 51,725 to 103,450 number of plays`

`<155,175 plays: Puzzles between 103,450 to 155,175 number of plays`

`<206,900 plays: Puzzles between 155,175 to 206,900 number of plays`

`<258,625 plays: Puzzles between 206,900 to 258,625 number of plays`

`>=258,625 plays: Puzzles with more than 258,625 number of plays`
<br/>

<h2>Data categories</h2>

- The Rating field consists of puzzle ratings from 545 to 3024. Rating Range was added to be split to 4 categories,  `<1200`, `<1800`, `<2200` and `>2200`. This is to easily identify beginner (<1200), intermediate (1200-1800), advanced (1800-2200) and expert (>2200) puzzles.  

- The Popularity field consists of puzzle ratings rated between -100 and 100. Popularity Range was added with 5 categories, `1 - Unpopular`, `2 - Disliked`, `3 - Mediate`, `4 - Liked` and `5 - Popular`.  

- The NbPlays field shows the number of plays the puzzle received. It consisted of number of plays ranging from 0 to 310341. NbPlays Range was added with 6 categories, `<51,725`, `<103,450`, `<155,175`, `<206,900`, `<258,625` and `>=258,625`. <br/>

<h2>Languages and Programs Used</h2>

- <b>Microsoft Excel (w/ Power Pivot Add-On)</b> <br />

<h2>Analysis Result</h2>

<p align="center">
Dashboard 1: <br/>
  <img src="https://user-images.githubusercontent.com/122200000/223697335-75f53db2-be85-4ec0-8eec-b9d8be3e5824.png" alt="Dashboard 1"/>
</p>
<br />

<br />
<p align="center">
Dashboard 2:  <br/>
<img src="https://user-images.githubusercontent.com/122200000/223697675-e2bce478-1762-412c-ab46-5706db45f95c.png" alt="Dashboard 2"/>
</p>
<br />

<br />
<p align="center">
Dashboard 3:  <br/>
<img src="https://user-images.githubusercontent.com/122200000/223699048-908d92b3-06fc-4eec-9d8d-f53fb5920c96.png" alt="Dashboard 3"/>
</p>
<br />


<h2>Discussions</h2>

- To begin with, across the puzzle rating ranges based on popularity range and number of plays, `<1800` puzzles have the most number of puzzles with a total of `1,270,692`. This is followed by `<1200` puzzles, `<2200` puzzles and `>=2200` puzzles with a total of `850,704`, `596,376` and `362,757` respectively.

- Next, across the popularity ranges based on the number of plays, `Popular` puzzles has the highest total of `2,861,397`. This is followed by `Liked`, `Mediate`, `Unpopular` and `Disliked` puzzles with a total of `150,934`, `30,306`, `22,835` and `15,057` respectively.

- It can also be seen that an overwhelming number of puzzles that are in the `popular` category have more number of plays. Most puzzles that are `unpopular`, `disliked`, `mediate` and `liked` tend to only get played less than `51,725` times.

- The highest number of popular puzzles from the rating range comes from `<1800` puzzles with a total of `1,270,692`. This is followed by `<1200` puzzles, `<2200` puzzles and `>=2200` puzzles with a total of `(850,704)`, `(596,376)` and `(362,757)`.

- Majority of the puzzles tend to get played less than `51,725` times with an overwhelming total of `3,079,850`. The remainder of `679` puzzles are played more than `103,450` times.

- Across the puzzle rating ranges, popular puzzles has the highest number of puzzles with total of `2,861,397`. This is followed by `liked`, `mediate`, `unpopular` and `disliked` with a total of `150,934`, `30,306`, `22,835` and `15,057` respectively.

- The top 3 themes that appear in puzzles shows a decent appearance across all puzzle rating ranges. Whereas, the top 3 themes that seldom appear in puzzles only appear in `0.02%` to `0.03%` of puzzles.
