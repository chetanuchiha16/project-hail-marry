# AI Graffiti Wall 🎨🖐️

AI Graffiti Wall is a real-time, gesture-controlled digital painting application. Using your computer's webcam and advanced hand-tracking technology, you can "spray" paint and erase on a virtual canvas simply by moving your hand in the air.

## ✨ Features

- **Real-time Hand Tracking**: Powered by MediaPipe for precise landmark detection.
- **Gesture-Based Painting**: Pinch your index finger and thumb together to start painting.
- **Gesture-Based Erasing**: Close your hand into a fist to toggle erasing mode.
- **Smooth Cursor Movement**: Implements Exponential Moving Average (EMA) for jitter-free drawing.
- **HUD (Heads-Up Display)**: Real-time feedback on current mode (IDLE, PAINTING, ERASING) and performance (FPS).
- **Clear Canvas**: Instantly wipe the canvas clean with a single keypress.

## 🚀 Getting Started

### Prerequisites

- **Python**: 3.10 or higher (Optimized for modern Python environments).
- **Webcam**: A functional internal or external camera.

### Installation

1. **Clone the repository**:
   ```bash
   git clone https://github.com/chetanuchiha16/project-hail-marry.git
   cd project-hail-marry
   ```

2. **Install dependencies**:
   It is recommended to use [uv](https://github.com/astral-sh/uv) for fast dependency management:
   ```bash
   uv sync
   ```
   Or using standard pip:
   ```bash
   pip install .
   ```

## 🎮 How to Use

Run the main application:
```bash
python src/ai_graffiti/main.py
```

### Controls

| Action | Gesture / Key |
| :--- | :--- |
| **Paint** | Pinch Index Finger and Thumb together 🤏 |
| **Erase** | Close hand into a Fist ✊ |
| **Move Cursor** | Move Index Finger (without pinching) ☝️ |
| **Clear Canvas** | Press `C` |
| **Quit** | Press `ESC` |

## 🛠️ Project Structure

- `src/ai_graffiti/main.py`: Entry point for the application. Orchestrates camera input and engine updates.
- `src/ai_graffiti/gesture_engine.py`: Handles hand landmark detection and gesture classification using MediaPipe.
- `src/ai_graffiti/painting_engine.py`: Manages the virtual canvas, drawing logic, and frame composition.
- `src/ai_graffiti/config.py`: Configuration for thresholds, colors, and smoothing factors.
- `src/ai_graffiti/contracts.py`: Data structures for state management.

## 📦 Dependencies

- **OpenCV**: For video processing and GUI.
- **MediaPipe**: For high-fidelity hand tracking.
- **NumPy**: For efficient canvas array manipulations.

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

---
Developed with ❤️ by [chetanuchiha16](https://github.com/chetanuchiha16)
