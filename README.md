# Chess-Game

## [chestboardjs](https://chessboardjs.com/index.html)

The code starts by creating a board and setting up the game. The positionCount variable is used to keep track of how many chess pieces are on the board. var pawnEvalWhite = [ [0.0, 0.0, 0.0, 0.0, 0.0, 0.0], [5.0, 5.0, 5.0, 5.0], [1., 1., 2., 3.]] var knightEval = [ [-5., -4., -3.]] var bishopEvalWhite = [ [-2., -1.]] var rookEvalWhite = [ [-2.]

The code creates a 2D array of points. The first row is the x-axis and the second row is the y-axis. Each point in the array represents an evaluation of white's king position. The first value in each point is black's evaluation of white's king position, and the second value is white's evaluation of black's king position. [2, 3] evaluates to 0 for both values because it falls on both axes (x and y). [1, 2] evaluates to -1 for both values because it falls on both axes (x and y). [3, 4] evaluates to -4 for white but +5 for black because it falls on only.

chessboard.js is a standalone JavaScript Chess Board. It is designed to be "just a board" and expose a powerful API so that it can be used in different ways. Here's a non-exhaustive list of things you can do with chessboard.js:

- Use chessboard.js to show game positions alongside your expert commentary.
- Use chessboard.js to have a tactics website where users have to guess the best move.
- Integrate chessboard.js and chess.js with a PGN database and allow people to search and playback games (see Example 5000)
- Build a chess server and have users play their games out using the chessboard.js board. 
##### using npm
```npm install @chrisoakman/chessboardjs```

##### using yarn
```yarn add @chrisoakman/chessboardjs```

##### using CDN
```<link rel="stylesheet"
      href="https://unpkg.com/@chrisoakman/chessboardjs@1.0.0/dist/chessboard-1.0.0.min.css"
      integrity="sha384-q94+BZtLrkL1/ohfjR8c6L+A6qzNH9R2hBLwyoAfu3i/WCvQjzL2RQJ3uNHDISdU"
      crossorigin="anonymous">
```

## Customizing your chesst pieces
The file path should be `img/chesspieces/wikipedia` with your chess pieces named as such:

- bK.png --> black king
- bQ.png --> black queen
- wK.png --> white knight
- wP.png --> white pawn
  
  
