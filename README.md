# Catch the Cat 🐱 (Web Edition)

A fast-paced, reaction-based clicker game. Originally prototyped in Scratch, this version has been rebuilt from the ground up using vanilla HTML, CSS, and JavaScript for smooth browser performance.

## 📁 Project Structure

*   `index.html` - The main game file containing the markup, styles, and game logic.
*   `cat.png` - The sprite for the target character *(Note: you will need to place your own image file in the same folder and name it this)*.

## 🚀 How to Play

1.  Download or clone this repository to your local machine.
2.  Ensure you have a `cat.png` image in the same folder as the HTML file.
3.  Double-click `index.html` to open it in your default web browser.
4.  Click **Start Game**.
5.  Click the cat before it moves! The cat will jump to random positions on the screen, waiting less time between jumps as the game goes on.
6.  Your Highscore is saved automatically to your browser's local storage.

## 🛠️ Customization & Modding

Want to tweak the game? Open `index.html` in any text editor (like VS Code or Notepad) and look for these sections:

*   **Change the Background Color:** Find `body` in the `<style>` section and change the `background-color` hex code.
*   **Change the Cat's Size:** Find `#cat` in the `<style>` section and adjust the `width` (currently `100px`).
*   **Adjust the Speed:** Scroll down to the `<script>` tag. In the `startGame()` function, change `catMovementLoop(1500)` to a lower number for a faster start, or a higher number for an easier start (1000 = 1 second).
*   **Change the Max Speed:** In the `catMovementLoop()` function, find `if (nextWaitTime < 500) nextWaitTime = 500;`. Lowering `500` makes the ultimate difficulty much harder.

## 🐛 Troubleshooting

*   **The cat is a broken image icon:** Make sure your image is exactly named `cat.png` and is in the exact same folder as `index.html`. If your image is a `.jpg` or `.svg`, simply change the `src="cat.png"` attribute inside the `<img>` tag in the HTML to match your file.
