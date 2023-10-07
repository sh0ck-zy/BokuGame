# Boku Game

**Boku** is a strategic board game played on a 10x10 hexagonal matrix where players aim to align five of their pieces in a row while also attempting capture moves. The game is winnable in six directions, providing a plethora of strategies and tactics for players to employ.

## Game Rules:

### Board:
- The board consists of a 10x10 matrix, with each cell having an associated coordinate.
- Given the hexagonal shape of the board:
  - The vertexes of the hexagon have 3 neighbors.
  - The edges of the hexagon have 4 neighbors.
  - All other cells have 6 neighbors.

### Objective:
- The primary goal for each player is to make a line of five of their pieces in any of the six winnable directions.

### Moves:
- Players take turns placing one of their pieces on an empty cell.
- If a capture move is available, players (whether human or AI) must execute the capture.
- After a successful "capture" move, where a player sandwiches two of their opponent's pieces, they get to remove one of the two "sandwiched" pieces.
  - The cell from which a piece was removed becomes "blocked" and is unavailable for the next move.

### Constraints:
- For a move to be valid, it must adhere to the following:
  - The chosen cell must be unoccupied.
  - The chosen cell must not be blocked from a previous capture.
  - It must be the player's turn. After a capture move, the player gets an additional turn to select an opponent's piece to remove.

### Additional Rules:
1. **Single Capture**: Players can capture only one piece per turn, even if multiple sequences of two contiguous pieces are flanked in a single move.
2. **Game Draw**: If the board is completely filled and neither player has achieved their win condition, the game ends in a draw.
3. **Forced Pass**: If a player has no legal moves (i.e., if all but one cell is occupied and this last cell was where a piece was captured in the previous move), the player must pass, allowing the opponent another turn.
4. **Threefold Repetition**: If the exact game state is repeated three times, indicating a potential infinite cycle of captures, the game ends in a draw. This situation is rare, and while it's advisable to implement, it's deemed unlikely to occur frequently.

## AI Opponent:

In this project, we've developed an AI opponent for the Boku game. The AI uses a combination of algorithms and heuristics to make decisions, ensuring a challenging gameplay experience.

- **Decision Making Algorithms**: Details about the implemented algorithms and their workings will be provided upon the completion of the game development.

---

For a comprehensive project planning and milestones, refer to [Project Planning](project-planning.md).
