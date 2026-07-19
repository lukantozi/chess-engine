# python-chess

A command-line chess game written in Python, with a computer opponent based on
minimax search and alpha-beta pruning.

Built as a learning project to practice object-oriented design, board-state
management, move validation, and basic adversarial search.

## Features

- Terminal-based board display using Unicode chess pieces
- Human-vs-AI play
- Coordinate move input, for example `e2e4`
- Object-oriented board and piece model
- Minimax-based AI with alpha-beta pruning
- Standard piece movement and captures
- Castling and pawn promotion
- Basic check and checkmate handling
- Save and resume support through `saved_game.json`

## Run

```sh
git clone https://github.com/lukantozi/chess-engine.git
cd chess-engine

python project.py
```

Enter moves in coordinate notation:

```text
Enter the move (eg. e2e4) or q to quit: e2e4
thinkning.......
Enter the move (eg. e2e4) or q to quit: q
You quit the game
```

## Project structure

| File | Purpose |
|---|---|
| `project.py` | Starts the game loop and handles player input |
| `board.py` | Represents and updates the chessboard state |
| `pieces.py` | Defines chess-piece behavior and movement rules |
| `ai.py` | Selects moves using minimax and alpha-beta pruning |
| `utils.py` | Shared helper functions |
| `test_project.py` | Tests for game behavior |

## Limitations

- The AI is intended as a learning implementation, not a competitive chess
  engine.
- This is a terminal application with no graphical interface.
- Invalid input is rejected; enter moves in coordinate notation such as `e2e4`.

## License

MIT
