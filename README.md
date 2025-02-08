# **Chess-Game**

A web-based interactive chess game built using **Chessboard.js**, a powerful JavaScript library for rendering chessboards with a dynamic and customizable API.

## **About Chessboard.js**
[Chessboard.js](https://chessboardjs.com/index.html) is a standalone JavaScript library designed to provide a simple yet flexible way to integrate chessboards into web applications. It is **not a chess engine**, but it can be combined with **Chess.js** to handle move validation, AI gameplay, and game logic.

### **Features & Use Cases**
- Display chess positions for **game analysis** and **expert commentary**.
- Create an **interactive tactics trainer** where users must guess the best move.
- Integrate **Chessboard.js** with **Chess.js** and a PGN database to allow users to **search, load, and replay games**.
- Build an **online chess server** where users can play games in real-time.

---

## **How the Code Works**
The code initializes a **chessboard** and sets up the game mechanics. A variable, `positionCount`, tracks the number of chess pieces on the board. 

### **Piece Evaluation System**
The game includes a **piece evaluation matrix** that assigns values to different board positions, influencing AI decision-making.

```javascript
var pawnEvalWhite = [ 
    [0.0, 0.0, 0.0, 0.0, 0.0, 0.0], 
    [5.0, 5.0, 5.0, 5.0], 
    [1.0, 1.0, 2.0, 3.0] 
];
var knightEval = [ 
    [-5.0, -4.0, -3.0] 
];
var bishopEvalWhite = [ 
    [-2.0, -1.0] 
];
var rookEvalWhite = [ 
    [-2.0] 
];
```
Each array represents **positional evaluations** for different pieces, guiding the AI in determining optimal placements.

### **King Position Evaluation**
The game evaluates White's **king position** based on a **2D point array**:

- The **first row represents the x-axis**.
- The **second row represents the y-axis**.
- Each point contains **two values**: 
  - **Black's evaluation of White's king position**.
  - **White's evaluation of Black's king position**.

**Examples:**
- `[2,3] → 0` for both players (neutral position).
- `[1,2] → -1` for both players (disadvantageous).
- `[3,4] → -4 for White, +5 for Black` (favorable for Black).

---

## **Installation**
You can install Chessboard.js using **npm, yarn, or CDN**.

### **Using npm**
```sh
npm install @chrisoakman/chessboardjs
```
### **Using yarn**
```sh
yarn add @chrisoakman/chessboardjs
```
### **Using CDN**
Add the following link in your HTML file:
```html
<link rel="stylesheet"
      href="https://unpkg.com/@chrisoakman/chessboardjs@1.0.0/dist/chessboard-1.0.0.min.css"
      integrity="sha384-q94+BZtLrkL1/ohfjR8c6L+A6qzNH9R2hBLwyoAfu3i/WCvQjzL2RQJ3uNHDISdU"
      crossorigin="anonymous">
```

---

## **Customizing Chess Pieces**
To use **custom chess pieces**, ensure that your image files are stored in the following directory:
```
img/chesspieces/wikipedia/
```
### **File Naming Conventions**
| Piece | Black (b) | White (w) |
|--------|-----------|-----------|
| King | `bK.png` | `wK.png` |
| Queen | `bQ.png` | `wQ.png` |
| Rook | `bR.png` | `wR.png` |
| Bishop | `bB.png` | `wB.png` |
| Knight | `bN.png` | `wN.png` |
| Pawn | `bP.png` | `wP.png` |

This allows seamless customization while maintaining compatibility with Chessboard.js.

---

## **Conclusion**
Chessboard.js is a powerful, flexible tool that allows developers to create **interactive chess experiences**. Whether you're building an **AI-powered chess engine**, a **chess training app**, or a **web-based multiplayer game**, Chessboard.js provides the foundation for an engaging and dynamic chess interface.

For advanced features such as **move validation, AI gameplay, and PGN parsing**, consider integrating Chessboard.js with **Chess.js**.

🚀 **Start building your chess game today!** ♟

