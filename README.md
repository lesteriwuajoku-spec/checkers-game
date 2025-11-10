# 🎲 Checkers Game in C++

A complete **text-based Checkers game** for two players, written in C++ as a college-level programming project. Features proper game logic, move validation, piece capturing, and king promotion.

## ✨ Features

### Core Gameplay
- ✅ **8x8 Checkers Board** - Traditional board layout
- ✅ **Two Players** - Red vs Black (alternating turns)
- ✅ **Move Validation** - Only legal moves allowed
- ✅ **Piece Capturing** - Jump over opponents to capture
- ✅ **King Promotion** - Pieces become Kings at opposite end
- ✅ **Win Detection** - Game ends when all pieces captured
- ✅ **Clear Visual Display** - Easy-to-read board with borders

### Game Rules Implemented
- Regular pieces move diagonally forward only
- Kings can move diagonally in any direction
- Capture by jumping over opponent pieces
- Multiple pieces can be captured in sequence
- Automatic king promotion
- Input validation and error handling

## 🔧 How to Compile & Run

### Windows:
```bash
g++ -std=c++11 -o checkers.exe checkers_simple.cpp
.\checkers.exe
```

### Mac/Linux:
```bash
g++ -std=c++11 -o checkers checkers_simple.cpp
./checkers
```

## 🎮 How to Play

### Piece Legend
- **r** = Red piece (moves up)
- **R** = Red King (moves any diagonal)
- **b** = Black piece (moves down)
- **B** = Black King (moves any diagonal)
- **::** = Empty playable square

### Making Moves
1. **Select a piece**: Enter row and column (e.g., `5 2`)
2. **Choose destination**: Enter target row and column (e.g., `4 3`)
3. **Cancel move**: Enter `-1 -1` to reselect piece

### Example Turn:
```
Current Player: RED
Select piece to move (row col): 5 2
Move to (row col) or (-1 -1 to cancel): 4 3
[Piece moves from position 5,2 to 4,3]
```

### Capturing Pieces
To capture an opponent's piece, **jump over it**:
```
From: 5 2 → To: 3 0
(Jumps over black piece at 4 1 and captures it)
```

### Becoming a King
When your piece reaches the **opposite end** of the board:
- Red reaches **row 0** → becomes **R** (King)
- Black reaches **row 7** → becomes **B** (King)

### Winning
Capture **all** of your opponent's pieces to win!

## 💡 C++ Concepts Demonstrated

### Core Programming Concepts
✅ **Classes & Objects** - Game encapsulation  
✅ **2D Arrays** - Board representation  
✅ **Functions** - Move validation, game logic  
✅ **Control Flow** - Game loop, conditionals  
✅ **Input Validation** - Error handling  
✅ **Boolean Logic** - Move legality checks  

### Data Structures
✅ **2D Array** (`int board[8][8]`) - Board state  
✅ **Integer encoding** - Piece types (0-4)  
✅ **State tracking** - Current player, piece counts  

### Algorithms
✅ **Diagonal move validation**  
✅ **Jump detection** (capture logic)  
✅ **King promotion logic**  
✅ **Win condition checking**  

## 📊 Code Structure

### Board Encoding
```
0 = Empty square
1 = Red piece
2 = Red king
3 = Black piece
4 = Black king
```

### Class Structure
The `CheckersGame` class contains:
- 2D array for board state
- Player tracking variables
- Piece count variables
- Methods for initialization, display, validation, and gameplay

## 🎓 Project Stats

- **Lines of Code**: ~350
- **Development Time**: 2-3 hours
- **Complexity**: Beginner-Intermediate
- **Files**: 1 (single file project)
- **Difficulty**: ⭐⭐⭐ (3/5)

## 📚 Skills Applied

- C++
- Object-Oriented Programming
- Data Structures (2D Arrays)
- Algorithm Design
- Input Validation
- Error Handling
- Software Testing

---

**Perfect for CS 135 students learning C++ fundamentals!** 🎓



