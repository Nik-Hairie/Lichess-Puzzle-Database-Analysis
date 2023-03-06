<h1>Data Analysis: Lichess Puzzle Database</h1>

<h2>Introduction</h2>
This is an analysis on Lichess Puzzle Database obtained from https://database.lichess.org/#puzzles. The database has over 3,080,529 chess puzzles to be analyzed. The puzzles database consists of fields as follows: PuzzleId, FEN, Moves, Rating, RatingDeviation, Popularity, NbPlays, Themes, GameUrl, OpeningFamily, OpeningVariation. Fields that were set aside includes PuzzleId, FEN, Moves, RatingDeviation, GameUrl, Opening Family and OpeningVariation. Data cleaning was performed on Rating, Popularity, NbPlays and Themes because it is relevant for the data analysis.

<h2>Abbreviations</h2>

- Puzzle Rating Range:

`<1200: Puzzles rating  below 1200`

`<1800: Puzzles rating between 1200 and 1800`

`<2200: Puzzles rating between 1800 and 2200`

`>=2200: Puzzles rating more than 2200`

- Puzzle Popularity Range:

`<51,725 plays: Puzzles with less than 51,725 number of plays`

`<103,450 plays: Puzzles between 51,725 to 103,450 number of plays`

`<155,175 plays: Puzzles between 103,450 to 155,175 number of plays`

`<206,900 plays: Puzzles between 155,175 to 206,900 number of plays`

`<258,625 plays: Puzzles between 206,900 to 258,625 number of plays`

`>=258,625 plays: Puzzles with more than 258,625 number of plays`


<h2>Data categories</h2>

- The Rating field consists of puzzle ratings from 545 to 3024. Rating Range was added to be split to 4 categories,  <1200, <1800, <2200 and >2200. This is to easily identify beginner (<1200), intermediate (1200-1800), advanced (1800-2200) and expert (>2200) puzzles.  

- The Popularity field consists of puzzle ratings rated between -100 and 100. Popularity Range was added with 5 categories, 1 - Unpopular, 2 - Disliked, 3 - Mediate, 4 - Liked and 5 - Popular.  

- The NbPlays field shows the number of plays the puzzle received. It consisted of number of plays ranging from 0 to 310341. NbPlays Range was added with 6 categories, <51,725, <103,450, <155,175, <258,625, <258,625 and >=258,625.
<br/>


<h2>Languages and Programs Used</h2>

- <b>Microsoft Excel (w/ Power Pivot Add-On)</b> 
<br />

<h2>Analysis Result</h2>

<p align="center">
Dashboard 1: <br/>
  <img src="https://user-images.githubusercontent.com/122200000/223208200-261d805c-d6be-42c2-aec2-d60ff9eed03f.png" alt="Dashboard 1"/>
</p>
<br />

<br />
<p align="center">
Dashboard 2:  <br/>
<img src="https://user-images.githubusercontent.com/122200000/223208495-362094a3-a322-42d9-a82c-3b8a5427d729.png" alt="Dashboard 2"/>
</p>
<br />
