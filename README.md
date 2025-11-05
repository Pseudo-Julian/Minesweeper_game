#  Minesweeper Game with AI

A classic **Minesweeper** game built with **Python** and **Pygame**, featuring an **AI player** that can make logical decisions and play automatically.

---

##  Features

- Interactive Minesweeper grid with mouse controls  
- AI that uses logic to deduce safe cells and mine locations  
- Visual interface built with `pygame`  
- Adjustable board size and number of mines  
- Smooth reset and restart system  

---

##  AI Logic

The AI is based on logical inference:
- It keeps a knowledge base of "sentences" representing the current state of the board.  
- Each sentence has a set of unknown cells and a count of how many of them contain mines.  
- From these, it deduces:
  - **Safe cells** — cells that are guaranteed not to contain a mine  
  - **Mines** — cells that must contain a mine  

When no safe move is known, the AI makes a **random move**.

---

##  Project Structure
```
Minesweeper_game/
├── assets/
│ ├── fonts/
│ │ └── OpenSans-Regular.ttf
│ └── images/
│ ├── flag.png
│ └── mine.png
├── minesweeper.py # Contains game logic and AI class
├── runner.py # Main game loop and UI built with pygame
├── requirements.txt # Dependencies
└── README.md # Project documentation
```

---
## Install dependencies
```
pip install -r requirements.txt
```
