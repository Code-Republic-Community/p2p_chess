
# Chess P2P

The project is a P2P chess that supports multiplayer mode.

During the development it was used:  
  • QT 6  
  • C++ 17
  
  ![Chess_Structure_UML vpd](https://user-images.githubusercontent.com/104615049/201946751-333e157b-5aa5-4bb1-8357-40f0bb93e6dd.png)

## Chess Board Description

Chess is played by two players on a chess board measuring eight-by-eight squares. The 64 squares alternate between light and dark colours - traditionally, black and white. When properly set up, a white square should be the rightmost square along the edge closest to each player.  
  
![Screenshot from 2022-11-15 17-25-54](https://user-images.githubusercontent.com/104615049/201948931-0240d211-cfd0-4f19-8491-2e912bd4b1f2.png)
  
Players’ pieces are set up in the two horizontal rows (known as ranks) closest to each player. The second rank - ie. the second row from the player’s perspective - consists of a line of eight pawns, each placed on a single square.
  
The closer rank is nearly symmetrical, with rooks (also known as castles) placed on the two leftmost and rightmost corner squares, followed by knights on the inside space next to them, then bishops.

The two central squares of the rank are occupied by the king and queen. The queen is placed on the square matching her colour (for example, the black queen on the black square), with the king occupying the remaining square of the opposite colour. This means that the king and queen of each colour face each other, making the correct setup symmetrical between the two players.

The white player takes the first move, with players alternating single turns until a player is defeated via checkmate or resigns. A draw can also be agreed. If playing with an optional timer, as in tournaments, the first player to run out of time forfeits the game.
## Basic Chess Rules

In chess, each player takes turns to make a single move. Players cannot choose to skip a turn - they must move a piece. Each chess piece moves in a specific way, and must be moved according to its legal movement.

![Screenshot from 2022-11-15 17-26-24](https://user-images.githubusercontent.com/104615049/201949346-6f658d2e-457b-44d2-9962-0e0d2f6466c6.png)

Except for the knight, which may jump over pieces, pieces cannot move through pieces of either colour without either stopping (in the same of a piece of the same colour) or capturing them (in the case of a piece of the opposite colour).

How to capture pieces
If a piece lands on a space with an opponent’s piece, that piece is captured and removed from the board. Pieces cannot be placed on the same square as a piece of the same colour. When a piece captures an opponent’s piece, it must finish its current move action and end the player’s turn.
## Figures Movement Rules

#### Pawn

Pawns move one square forward in a straight line. They cannot move horizontally, diagonally or backwards.

An exception to this is if a pawn is yet to be moved during the game. If a pawn has not yet moved, it may be moved two squares forward as a single move. Both squares must be empty. The player can also choose to move the piece a single square.

The only time a pawn may move diagonally is when capturing an opponent’s piece. Pawns may capture an opponent’s piece on either of the diagonal spaces to the left or right ahead of the piece. As part of capturing the piece, the pawn will move diagonally to replace the captured piece. A pawn cannot capture an adjacent piece on any other square, or move diagonally without capturing.

#### Rook (Castle)

The rook, sometimes called the castle, can move any number of squares horizontally along its current row (rank) or column (file). It cannot pass through pieces of the same colour, and can capture pieces of the opposite colour by moving onto an occupied space. It cannot move diagonally for any reason.

#### Knight

Knights are the only chess piece that may be moved ‘through’ other pieces by ‘jumping’ over them. It captures pieces as normal by landing on a space occupied by a piece of the opposite colour and cannot move to a square occupied by a piece of the same colour, but may move over pieces of either colour during its move.

Knights move in a fixed ‘L’ pattern: two squares forward, backward, left or right, then one square horizontally or vertically, or vice versa - one square forward, backward, left or right, followed by two squares horizontally or vertically to complete the ‘L’ shape.

This means that the knight can always move to the closest square that is not on its current row (rank), column (file) or directly adjacent diagonally.

The knight must move the full distance - it cannot move just two squares in a straight line without also moving one to the side, for instance.

#### Bishop

The bishop can move any number of squares diagonally - this means it always moves along the diagonal line of squares matching the current colour of its square. This means that each player begins the game with one bishop that can move on each colour. A bishop cannot move horizontally or vertically for any reason. It cannot move through pieces of the same colour, and captures a piece of the opposite colour by moving onto its square.

#### Queen

The queen may move any number of squares horizontally, vertically or diagonally. These movements must be made in a single straight line during a single turn. (In other words, you can’t move three squares diagonally, followed by three spaces vertically.) The queen cannot move through pieces of the same colour, and captures a piece of the opposite colour by moving onto its square.

#### King

The king moves a single space horizontally, vertically or diagonally. The king cannot move into a space that would grant a check or checkmate to the opponent player.

As an exception to all other chess pieces, the king is never captured - a player loses the match when the king is placed into checkmate, which would lead to an unavoidable capture on the opponent’s next turn.
## What is check and checkmate?

When a piece moves in a way that would allow a player to capture the opponent’s king on their next turn, the attacking player typically announces “check”.

The player placed into check must move their king or move another piece to stop the attack on their next turn - either by blocking the move or capturing the attacking piece.

If a player creates a situation where their opponent cannot stop their king from being captured on the next turn, the attacking player announces “checkmate” and immediately wins the game. The king is never captured - a game of chess is won when a successful checkmate is announced.

![photo_2022-11-15_17-37-12](https://user-images.githubusercontent.com/104615049/201949421-3a8b61c3-0ed3-4418-b3fe-ccfad313ce23.png)

A player can also choose to resign, granting their opponent the victory. Matches can also end in an agreed draw - for example, as the result of stalemate leaving a player without any legal moves, or if no player can win using available legal moves, a situation known as a “dead position”. One example of a dead position is when both players are left with their king as their only remaining piece on the board.

Draws can also occur as the result of advanced rules typically used in professional tournaments, including identical board positions occurring three or five times - rules known respectively as threefold repetition and fivefold repetition - or no captures or pawn moves taking place within the last 50 or 75 moves. The exact rules used can depend on the tournament and agreement between the players.


## Advanced Chess Rules

There are a number of advanced rules that can be used in chess, along with specific openings and board positions known by a variety of names, from the Double King's Pawn Opening to the famous King’s Gambit and Queen’s Gambit.

Advanced rules can include specific variants that alter the core rules of the game, along with surrounding requirements often used in tournament settings, such as timing and the touch-move rule - which states that once a piece is touched by a player, it must make a legal move.

As this is a beginner’s guide to learning chess, we’ll only be covering some of the essential advanced rules here - rules that should always be used in conjunction with the basic rules for moving and capturing pieces, as well as the standard setup and rules for declaring checkmate.

Once you know the basics of how to play chess, there are hundreds of books and other resources out there to help you discover the deep strategy and near-endless variations possible during games - as well as local tournaments that can help you refine your play and tactics.


### How to promote a pawn
If a pawn reaches the opposite edge of the board - the farthest row (rank) from the controlling player - it is promoted to another piece: a rook, knight, bishop or queen. The new piece replaces the pawn on its current square, and follows the movement rules for the respective piece.

While most casual players use captured pieces to represent promoted pieces, a pawn can legally be promoted to any piece regardless of whether it has been captured. For example, a player may have multiple queens as the result of promoting pawns, or multiple bishops able to move along diagonal lines of the same colour depending on the square on which the pawn was promoted.

There is no limit to the number of pawns that can be promoted.

### What is En passant?
En passant - French for ‘in passing’ - is one of the most famous moves in chess. En passant occurs when a pawn moves two squares forward as the result of its optional starting move.

If an opponent’s pawn would have been able to legally capture the moving pawn had it only moved one square instead of two, the opponent can declare en passant on their next turn and move their pawn diagonally onto the square that the pawn passed through - capturing the pawn as if it had only moved one square.

En passant must be declared and made as the opponent’s next turn to be legal - otherwise, the player with the chance to capture the pawn loses the opportunity.

### What is Castling?
Castling is perhaps the most complicated basic rule in chess, and a rule that many beginners often overlook as a result.

Castling is permitted when a player’s king piece and a rook have not yet moved during the game. Castling can be performed with either rook, as long as they haven’t moved - in other words, they are still in their starting corners on the edge closest to the controlling player.

Castling involves a player moving the king piece two squares towards the rook with which they are castling, before moving the rook to the square that the king moved ‘through’. This effectively puts the rook adjacent on the other side of the king, while the king moves two squares towards the space in which the rook started the game. Regardless of whether castling is performed with the rook closer to the king (kingside) or one square further away (queenside), the king only ever moves two spaces.

The king cannot be used in a castling manoeuvre if it is currently in check, but a rook can be used in castling even if it is under threat from an opponent’s piece - in other words, if it could be captured on the opponent’s next turn, or on any of the squares it passes through while performing the move.

As usual, castling cannot be used to move the king if it would put the king into check. Castling also cannot be used if there are any pieces between the king and the rook - the squares between must be clear.
## Gameplay Description

The chess program is intuitive and understandable for beginners.

When you click on a figure, the trajectory of its movement appears.
Each player has a visible analogous timer for counting the game time. The standard is 1 hour.

Each player can only control pieces of his own color, sequentially.

When one of the players runs out of time, a loss is automatically declared.

At the end of the game with any outcome, the players will see a screen informing them of their status, that is, whether the player has lost or won.
## Multiplayer Description

When you turn on the program, a game room is created, to which the next connecting player is automatically added.

After connecting, the first player sees a waiting screen.

![Screenshot from 2022-11-15 17-29-04](https://user-images.githubusercontent.com/104615049/201949584-5747c445-6196-4a2e-9984-17a3426dcdc1.png)

The move is transmitted sequentially, depending on whether you have connected to an existing room or a new one has been created for you. This simulates the randomness of the color selection.

The program supports the simultaneous connection of a large number of players.
