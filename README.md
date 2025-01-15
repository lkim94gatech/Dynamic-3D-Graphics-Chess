# Dynamic 3D Graphics Chess

This project is a dynamic 3D chess simulation built in **C++** using **OpenGL** and supporting libraries. The application allows users to interact with a 3D chessboard, manipulate the camera, and toggle lighting effects. It showcases the use of **lighting**, **shading**, **model transformations**, and **keyboard inputs** for a realistic 3D graphics application.

---

## Objective

To understand and apply **3D graphics rendering** techniques such as loading 3D models, using shaders, and implementing user interactions.

---

## Features

1. **3D Rendering**:
   - Displays a fully modeled chessboard and pieces using `.obj` files.
   - Implements realistic lighting and shading for visual effects.

2. **Camera Controls**:
   - `W`/`S`: Move the camera closer to or farther from the origin.
   - `A`/`D`: Rotate the camera left or right while maintaining distance.
   - Up/Down Arrow Keys: Rotate the camera up or down radially.

3. **Lighting Toggles**:
   - `L`: Toggle specular and diffuse lighting components while maintaining ambient light.

4. **Exit**:
   - Press the `Escape` key to close the window and exit the program.

---

## File Structure

### Core Files
- **chess_3D_view.cpp**: Main application file that initializes OpenGL, handles user inputs, and manages the rendering loop.
- **chessComponent.cpp**: Defines the `chessComponent` class for handling individual chess piece models.
- **chessCommon.h**: Common constants and macros used across the project.
- **StandardShading.vertexshader** and **StandardShading.fragmentshader**: GLSL shaders for rendering.

### Assets
- **3D Models**:
  - `Chess/chess-mod.obj`: Contains the 3D models of the chess pieces.
  - `Stone_Chess_Board/12951_Stone_Chess_Board_v1_L3.obj`: Contains the 3D model of the chessboard.

- **Textures**:
  - `Stone_Chess_Board/*.bmp`: Textures for the chessboard.
  - `Chess/*.bmp`: Textures for the chess pieces.

---

## Classes

### 1. **chessComponent**
   - Manages individual chess piece models, including loading, transformations, and rendering.
   - Handles OpenGL buffer creation and texture setup.

---

## How to Run

### Prerequisites
- **OpenGL**: Installed on your system.
- **GLEW**: For managing OpenGL extensions.
- **GLFW**: For creating windows and handling user input.

### Steps
1. Clone the repository:
   ```bash
   git clone <repository_url>
   cd Chess3DSimulation
   ```
2. Build the Project Using CMake:
   ```bash
   cmake --build .
   cmake ..
   ```
3. run the executable:
   ```bash
   ./chess3D
   ```

## Gameplay Instructions

### Controls:
- **W/S**: Move the camera closer to or farther from the origin.
- **A/D**: Rotate the camera left or right.
- **Up/Down Arrow Keys**: Rotate the camera up or down.
- **L**: Toggle lighting components on or off.
- **Escape**: Exit the simulation.

### Objective:
- View and interact with the 3D chessboard and pieces using camera controls.

### Graphics:
- The chessboard and pieces are rendered with textures and lighting effects for added realism.

---

## Testing and Debugging

### Key Features to Test:

1. **3D Model Loading**:
   - Ensure all `.obj` files for the chess pieces and board load correctly without errors.

2. **Lighting Effects**:
   - Verify that lighting toggles correctly when the **L** key is pressed.

3. **Camera Movements**:
   - Test all camera controls to ensure smooth movement and rotation:
     - **W/S** for zooming in and out.
     - **A/D** for left/right rotation.
     - **Up/Down Arrow Keys** for vertical rotation.

4. **Rendering**:
   - Confirm that all chess pieces and the board are rendered at the correct positions and scaling.


