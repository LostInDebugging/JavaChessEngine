# JavaChessEngine
A chess engine in Java... written by me!

## The `Game` Class
This is the class that handles the basic functionality of the game.

### Methods of the `Game` class
```
// The 2 constructors for the Game class
// load the starting position if a FEN string is not given
Game()

Game(String FEN)

// Changes the state of an existing game
public void LoadFEN(String FEN)

// Returns a FEN string constructed from the current game state
public String ExportFEN()

// Make a move in the game (given a move in standard move notation)
public void MakeMove(String move)

// Get a list of all possible moves in the current position (standard move notation)
public List<String> GetMoveList()

// Undo the last n moves of the game
public void UndoLastNMoves(int n)
```

### Example Usage
```
Game g = new Game(); // creates a game with the default starting position
g.MakeMove("d4");
List<String> moves = g.GetMoveList();
```
