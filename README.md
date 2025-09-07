# EduChess

<img width="1134" height="460" alt="image" src="https://github.com/user-attachments/assets/7ba51378-d4bf-4e22-a08d-3fa601f9d6d6" />



**EduChess** is an educational chess assistant developed by the **Rook and Rule** team.  
It uses **computer vision and machine learning** to detect a chessboard from images, convert it into FEN notation, and let you play against the **Stockfish chess engine** with real-time feedback and move explanations.  

---

## Features

- 🎥 **Board Detection** – Detects chessboards from images using OpenCV.  
- ♟ **Piece Recognition** – Identifies chess pieces and their colors with trained PyTorch models.  
- 📝 **FEN Conversion** – Generates Forsyth–Edwards Notation (FEN) to represent the board state.  
- 🤖 **Engine Integration** – Plays against the Stockfish engine with adjustable difficulty.  
- 💬 **Move Feedback** – Provides real-time analysis and comments on player moves.  
- 🖥 **GUI** – Visualizes the game and assists players interactively.  

---

## Repository Structure
EduChess/
|-- board_detection.py # Detects the chessboard and extracts squares
|-- get_position.py # Uses models to detect pieces & colors, outputs FEN
|-- comments.py # Explains and rates moves
|-- GUIPlayer.py # Graphical interface and interaction
|-- arm_vs_arm.py # Stockfish vs Stockfish for data generation
|-- models/ # Pretrained PyTorch models for detection

---

## Dataset & Models

- Chess piece dataset (Zenodo):  
  [https://zenodo.org/records/6656212](https://zenodo.org/records/6656212)

---  
  
## Stockfish Engine

Download the latest Stockfish engine here:  
👉 [https://stockfishchess.org/download/](https://stockfishchess.org/download/)  

Place the executable inside a `stockfish/` folder in the project directory.  

---

EduChess is a derivative of [ChessEduBotArm](https://github.com/RooKAndRule/ChessEduBotArm), focusing on the core assistant functionality of board detection, FEN conversion, Stockfish play, and real-time feedback, while ChessEduBotArm represents the future vision of the project, integrating a robotic arm and LSTM models to predict the next move, track whether the player is improving or repeating mistakes, and evaluate how well the prediction model itself performs.




  
