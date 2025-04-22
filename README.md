# TicTacToe_with_AI
This project implements an intelligent Tic-Tac-Toe game using the Minimax algorithm and 
its optimized version, Alpha-Beta Pruning, in Python. The game includes a user-friendly 
GUI where a human player competes against an AI that always plays optimally. 
The key goals of this project: 
 Understand and implement the Minimax algorithm. 
 Apply Alpha-Beta Pruning to improve performance. 
 Integrate both into a GUI-based Tic-Tac-Toe game. 
 Compare performance of basic Minimax vs. Alpha-Beta pruning. 
�
� 2. Algorithms Used 
➤ Minimax Algorithm 
 A recursive decision-making algorithm used in two-player games. 
 Explores all possible game moves to select the best one. 
 Assumes opponent also plays optimally. 
 Time complexity: O(b^d), where b is branching factor and d is depth. 
➤ Alpha-Beta Pruning 
 An enhancement of Minimax that prunes branches that won’t influence the result. 
 Greatly reduces computation time. 
 Best-case time complexity: O(b^(d/2)). 
�
� 3. Code Structure 
�
� tictactoe_ai.py – Game logic and AI 
 TicTacToe class: 
o Handles board state, moves, win/draw detection. 
 AlphaBetaAI class: 
o Uses Minimax with Alpha-Beta Pruning to select optimal AI moves. 
�
� tictactoe_gui.py – Graphical User Interface (GUI) 
 Built using Tkinter. 
 3x3 clickable grid. 
 Human plays 'X', AI plays 'O'. 
 Winner/draw messages shown via popup. 
 Colored and centered grid with resizable layout. 
�
� 4. GUI Features 
 Centered layout with clean, minimal design. 
 Button colors: 
o ‘X’ = Blue 
o ‘O’ = Green 
 Responsive UI: AI responds after a short delay. 
 Automatically disables board after game ends. 
⚙
 ️ 5. How the Game Works 
1. Human plays first as X. 
2. Each move triggers the AI using Alpha-Beta Pruning. 
3. The board checks for a win/draw after each turn. 
4. On win or draw, a popup message appears, and input is disabled. 
�
� 6. Minimax vs Alpha-Beta (Performance Notes) 
Criteria 
Nodes explored 
Speed 
Optimal Move Selection Yes 
Efficiency 
Minimax 
High 
Slower 
Alpha-Beta Pruning 
Fewer (due to pruning) 
Faster 
Yes 
Low for depth > 4 Much better 
Alpha-Beta Pruning drastically reduces the number of recursive calls while returning the 
same optimal results as Minimax. 
�
� 7. Requirements 
 Python 3.x 
 Tkinter (usually comes pre-installed) 
 Run tictactoe_gui.py to launch the game.
