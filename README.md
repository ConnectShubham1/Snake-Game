# Snake-Game
A classic snake game developed using Java Swing.
# Snake Game

## Description

A classic snake game developed using Java Swing.

## How to Run

1. **Compile the Java files**:
    ```
    javac src/SnakeGame.java src/GamePanel.java src/Snake.java src/Apple.java
    ```

2. **Run the SnakeGame**:
    ```
    java -cp src SnakeGame
    ```

3. **Follow the prompts**:
    - Use arrow keys (up, down, left, right) to control the snake.
    - Try to eat the red apples without colliding with the walls or yourself.
    - The game ends when you collide with the wall or yourself.

## Example Code

### SnakeGame.java

```java
import javax.swing.*;

public class SnakeGame {
    public static void main(String[] args) {
        JFrame frame = new JFrame("Snake Game");
        frame.setDefaultCloseOperation(JFrame.EXIT_ON_CLOSE);
        frame.setResizable(false);

        GamePanel gamePanel = new GamePanel();
        frame.getContentPane().add(gamePanel);

        frame.pack();
        frame.setLocationRelativeTo(null);
        frame.setVisible(true);

        gamePanel.startGame();
    }
}
