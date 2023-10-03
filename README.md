# Checkers
The project involved the development of a two-player board game, which appeared to be a digital implementation of Checkers or a similar board game. The project can be divided into two main components: technical implementation and user interface enhancements. Here's a description of the project with a focus on technical details:

**Technical Implementation:**
1. **Initial Display and Piece Sprites:** The project began with the creation of graphical elements (sprites) to represent the game board and its pieces.

2. **PS/2 Interrupts:** One team member analyzed the DE1-Soc board manual to configure PS/2 interrupts and set up interrupt handling in C. This involved setting up stack pointers for interrupt mode and defining an interrupt service routine (ISR). The ISR read input from the PS/2 port and called corresponding functions based on arrow key inputs for movement and enter key inputs for selection.

3. **Game Logic:** The other team member focused on implementing the game's logic, which included:
   - Determining valid moves for selected pieces, considering diagonal blocks and jumps over opponents.
   - Handling jump sequences, including recursive checks for multiple jumps.
   - Resolving takes or kills during a move, considering all possible combinations of movements.
   - Tracking when a piece should become a king piece when reaching the opposite border.
   - Implementing king piece movements and valid jump directions.

4. **Scoring Functionality:** The game included a scoring system where players incrementally increased their kill counts after performing takes or kills. The first player to reach a kill count of 12 was declared the winner.

5. **Bug Fixing:** Ongoing work involved identifying and fixing bugs and edge cases to ensure smooth gameplay.

**User Interface Enhancements:**
1. **UI Improvements:** The UI was enhanced with a wooden finish background for the game board, creating a more visually appealing appearance. The piece sprites were also updated to match the board's aesthetics.

2. **Starting Page:** A starting page was implemented, allowing the game to commence only when the user pressed the space bar, ensuring a controlled game start.

3. **Character Buffer:** A live score count was displayed using a character buffer, providing real-time feedback on the game's progress.

4. **Status Bar:** A status bar was introduced to indicate whose turn it was during the game.

5. **Game Ending Integration:** The logic for determining the game's end and the winning player was connected to the UI. An ending screen displayed the winning player's number when the game concluded.

Overall, the project combined technical programming skills with user interface design to create a functional and visually appealing two-player board game with detailed game logic and a polished user experience.