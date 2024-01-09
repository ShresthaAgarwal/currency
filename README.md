# Eye - Mouse

## Introduction
This Python script utilizes computer vision and facial landmark detection to create an eye-controlled mouse. The program tracks specific facial landmarks associated with the eyes and performs mouse movements and clicks based on the detected positions.

## Requirements
- Python 3.x
- OpenCV (`pip install opencv-python`)
- Mediapipe (`pip install mediapipe`)
- PyAutoGUI (`pip install pyautogui`)

## Usage
1. Install the required dependencies.
2. Connect a webcam to your computer.
3. Run the script.

## How it Works
The script captures video from the webcam, detects facial landmarks using Mediapipe's FaceMesh, and extracts relevant eye landmarks. It then calculates screen coordinates based on these landmarks and uses PyAutoGUI to control the mouse. A mouse click is simulated when certain conditions (e.g., specific eye movements) are met.

## Configuration
- `cam = cv2.VideoCapture(0)`: Set the parameter of `VideoCapture()` to the index of your desired camera.
- `face_mesh = mp.solutions.face_mesh.FaceMesh(refine_landmarks=True)`: Configures the FaceMesh model with refined landmarks.
- Adjust the conditions for mouse clicks based on the calculated differences in landmark positions.

## Dependencies
- [OpenCV](https://github.com/opencv/opencv)
- [Mediapipe](https://github.com/google/mediapipe)
- [PyAutoGUI](https://github.com/asweigart/pyautogui)

## License
This project is licensed under the [MIT License](LICENSE).

## Acknowledgments
- The project uses OpenCV, Mediapipe, and PyAutoGUI libraries.
- Inspired by the idea of gaze-based mouse control.

Feel free to customize this README according to your project's specifics and any additional information you'd like to provide.

