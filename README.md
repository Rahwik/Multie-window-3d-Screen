# Window Manager with Animated Cubes

## Overview
This project features a dynamic window management system with animated cubes positioned based on the layout of active windows. Utilizing **Three.js** and **WebGL**, this interactive system renders cubes that move and rotate smoothly based on the position of windows on the screen. The cubes dynamically adjust their size, color, and movement as the window setup changes, creating a visually stunning and responsive effect that reacts to user interactions.

---

## Features
- **Responsive Window Management**: Tracks the position and size of browser windows in real-time.
- **Smooth Transitions**: Cubes follow window changes with visually appealing easing effects.
- **Dynamic Cube Positioning**: The cubes' positions update dynamically to reflect windows' layout changes.
- **Customizable**: Highly extensible with hooks to add custom window metadata and interactions.
- **Three.js Based**: Ensures smooth and efficient 3D rendering.

---

## Installation

### Prerequisites
To run this project, ensure the following are installed:
- [Node.js](https://nodejs.org/) (v14 or higher)
- npm (or Yarn)

### Steps

1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/window-manager-cubes.git
   cd window-manager-cubes
   ```

2. Install dependencies:
   ```bash
   npm install
   ```

3. Run the application:
   ```bash
   npm start
   ```

4. Open your browser and navigate to [http://localhost:3000](http://localhost:3000) to view the project.

---

## How It Works

### 1. **Window Management**
- Listens to window events and tracks changes in their position and size using the `WindowManager` class.
- Automatically updates cubes to reflect changes in the windows' layout.

### 2. **Scene Setup**
- A **Three.js** scene is initialized with an orthographic camera, providing a 3D environment for the cubes.
- Smooth transitions and rotational animations enhance the cubes' movement.

### 3. **Cubes' Behavior**
- Dynamically sized and positioned based on the number and layout of windows.
- Re-generates cubes as windows are added or removed, updating the scene accordingly.

### 4. **Smooth Easing**
- Uses `sceneOffset` for smooth scrolling effects when windows move.
- Falloff values ensure fluid and visually pleasing animations.

---

## Project Structure
```
/window-manager-cubes
├── /src
│   ├── WindowManager.js       # Core window manager logic
│   ├── index.html             # HTML file for rendering the application
│   └── main.js                # Main entry point for 3D rendering logic
├── /assets                    # Static assets (images, fonts, etc.)
├── package.json               # npm package configuration file
└── README.md                  # Project documentation
```

### Key Files
- **`WindowManager.js`**: Manages window interactions and stores metadata for each window instance.
- **`main.js`**: Initializes the Three.js scene, renderer, camera, and manages the cubes.
- **`index.html`**: Provides the basic HTML structure and canvas for rendering the scene.

---

## Configuration
You can customize various aspects of the system:

### 1. **Window Shape**
Modify the appearance and behavior of windows by interacting with the `WindowManager` instance.

### 2. **Cubes' Appearance**
Adjust cube sizes, colors, and rotations by tweaking parameters in `main.js`.

### 3. **Rendering Settings**
Fine-tune the WebGL renderer's settings, such as pixel ratio and antialiasing, for optimal visual quality.

---

## Developer Notes
- Built with **Three.js** for efficient 3D rendering.
- The `WindowManager.js` module is modular and reusable for other projects.
- Includes a responsive design with automatic scene resizing to fit browser dimensions.
- Cubes' colors are dynamically generated using **HSL (Hue, Saturation, Lightness)**, ensuring visually distinct and vibrant animations.

---

## Contributing
We welcome contributions to improve this project! To contribute:

1. Fork the repository.
2. Clone your fork to your local machine:
   ```bash
   git clone https://github.com/yourusername/window-manager-cubes.git
   ```
3. Create a new branch for your changes:
   ```bash
   git checkout -b feature-name
   ```
4. Make your changes and commit them with clear messages.
5. Push your changes to your fork:
   ```bash
   git push origin feature-name
   ```
6. Submit a pull request with a detailed description of your changes.

---

## License
This project is licensed under the **MIT License**. See the [LICENSE](./LICENSE) file for details.

---

## Acknowledgments
- **Three.js**: For providing an excellent 3D rendering library.
- Community contributions for feedback and feature suggestions.

Feel free to reach out with any questions or suggestions to improve the project!

