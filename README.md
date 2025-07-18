# 2048 Game

A Java implementation of the popular 2048 puzzle game using the Processing library for graphics and Gradle as a dependency manager.

## 🎮 Game Description

2048 is a single-player sliding block puzzle game. The game's objective is to slide numbered tiles on a grid to combine them to create a tile with the number 2048. The game is won when a tile with a value of 2048 appears on the board.

## ✨ Features

- **Classic 2048 Gameplay**: Slide tiles to combine matching numbers
- **Customizable Grid Size**: Play with different board sizes (2x2 to 7x7)
- **Smooth Animations**: Beautiful tile movement and merge animations
- **Visual Feedback**: Hover effects and color-coded tiles
- **Score Tracking**: Current score and best score display
- **Timer**: Track your game duration
- **Game Over Detection**: Automatic game over detection when no moves are possible
- **Modern UI**: Clean, intuitive interface with proper color scheme

## 🛠️ Technology Stack

- **Java 8**: Core programming language
- **Processing 3.3.7**: Graphics library for rendering and user interaction
- **Gradle**: Build system and dependency management
- **JUnit 5**: Unit testing framework

## 📋 Prerequisites

- Java 8 or higher
- Gradle (optional - wrapper is included)

## 🚀 Installation & Setup

1. **Clone the repository**:
   ```bash
   git clone <repository-url>
   cd 2048-Game
   ```

2. **Build the project**:
   ```bash
   gradle build
   ```

3. **Run the game**:
   ```bash
   gradle run
   ```

   Or with a custom grid size:
   ```bash
   gradle run --args="7"
   ```

## 🎯 How to Play

### Controls
- **Arrow Keys**: Move tiles in the corresponding direction
- **Mouse Click**: Click on empty cells to place random tiles (2 or 4)
- **WASD Keys**: Alternative movement controls (W=Up, A=Left, S=Down, D=Right)

### Game Rules
1. Tiles slide in the direction of the arrow key pressed
2. When two tiles with the same number collide, they merge into one tile with the sum of their values
3. After each move, a new tile (2 or 4) appears in a random empty cell
4. The game ends when no more moves are possible
5. The goal is to create a tile with the value 2048

### Scoring
- Points are awarded for each merge
- The score is the sum of all merged tile values
- Your best score is automatically saved

## 🏗️ Project Structure

```
2048-Game/
├── src/
│   └── main/
│       ├── java/
│       │   └── TwentyFortyEight/
│       │       ├── App.java          # Main game class with Processing setup
│       │       └── Cell.java         # Individual tile/cell implementation
│       └── resources/
│           └── TwentyFortyEight/
│               └── 8.png             # Game assets
├── build.gradle                      # Gradle build configuration
└── README.md                         # This file
```

## 🎨 Key Components

### App.java
- Main game logic and Processing framework integration
- Handles user input (keyboard and mouse)
- Manages game state (score, timer, game over)
- Implements tile movement algorithms
- Renders UI elements (score display, timer, game over screen)

### Cell.java
- Represents individual tiles on the game board
- Handles tile animations (movement, spawn, merge)
- Manages tile appearance and color schemes
- Implements visual effects and hover states

## 🎮 Game Features in Detail

### Customizable Grid Size
The game supports different board sizes from 2x2 to 7x7. The maximum size is limited to 7x7 to ensure the game board fits comfortably on most desktop screens. You can specify the size when launching:
```bash
gradle run --args="7"  # 7x7 grid
```

### Smooth Animations
- **Movement Animation**: Tiles smoothly slide to their destination
- **Spawn Animation**: New tiles appear with a subtle scale effect
- **Merge Animation**: Merged tiles briefly scale up to emphasize the combination

### Visual Design
- **Color-coded Tiles**: Each tile value has its own distinct color
- **Hover Effects**: Tiles brighten when the mouse hovers over them
- **Modern UI**: Clean score display with rounded rectangles
- **Responsive Layout**: Adapts to different grid sizes

### Game Logic
- **Intelligent Movement**: Tiles merge correctly and slide as far as possible
- **Random Tile Generation**: New tiles appear in random empty cells
- **Game Over Detection**: Automatically detects when no moves are possible
- **Score Calculation**: Tracks points for each successful merge

## 🧪 Testing

Run the test suite:
```bash
gradle test
```

## 📦 Building JAR

Create an executable JAR file:
```bash
gradle jar
```

The JAR file will be created in `build/libs/` and can be run with:
```bash
java -jar build/libs/2048-Game-1.0.jar
```

## 🎯 Future Enhancements

Potential improvements for future versions:
- Save/load game state
- Undo functionality
- Different themes and color schemes
- Sound effects
- High score leaderboard
- Touch support for mobile devices
- AI solver demonstration

## 🤝 Contributing

1. Fork the repository
2. Create a feature branch
3. Make your changes
4. Add tests for new functionality
5. Submit a pull request

## 📄 License

This project is open source and available under the [MIT License](LICENSE).

## 🙏 Acknowledgments

- Original 2048 game by Gabriele Cirulli
- Processing library for graphics and interaction
- Gradle team for the build system

---

**Enjoy playing 2048!** 🎮