# Chess-Game

## [chestboardjs](https://chessboardjs.com/index.html)

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
  
  