# Camera-Surveillance-System

# Face Registration and Surveillance System

This project implements a **Face Registration and Surveillance System** using Python. It combines real-time object detection and face recognition to enhance security monitoring. The system includes motion-triggered surveillance, face registration functionality, and a user-friendly GUI for seamless interaction.

## Features

- **Real-time Object Detection**: Utilizes the YOLO model for accurate object detection with GPU support.
- **Face Registration and Recognition**: Detects, registers, and recognizes faces using the Face Recognition library.
- **Motion Detection**: Activates surveillance mode upon detecting significant motion in the camera feed.
- **GUI Integration**: User-friendly interface for face registration and starting surveillance, built with Tkinter.
- **Dynamic Bounding Boxes**: Displays labeled bounding boxes for detected objects and recognized faces.

## Prerequisites

Ensure the following dependencies are installed before running the application:

- Python 3.8 or higher
- OpenCV (`cv2`)
- Face Recognition library
- Tkinter (built into Python)
- PyTorch and Ultralytics YOLO

Install required Python packages using the following command:
```bash
pip install opencv-python face-recognition ultralytics torch

## Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/your-username/face-surveillance-system.git
   cd face-surveillance-system
   ```

2. Download the YOLO model weights (e.g., `yolov8n.pt`) from the [Ultralytics YOLO repository](https://github.com/ultralytics/ultralytics).

3. Place the YOLO model weights in the project directory.

## How to Use

### 1. Run the Application
Start the application by executing:
```bash
python main.py
```

### 2. Face Registration
- Enter a name in the GUI and press the **Register Face** button.
- Point the camera at the face to register and press **'c'** to capture.
- If the face is successfully registered, it will be saved with the entered name.

### 3. Start Surveillance
- Click the **Start Surveillance** button in the GUI.
- The system will detect motion, start object detection, and recognize registered faces.
- Press **'q'** to exit surveillance mode.

### 4. GUI Controls
- The GUI provides buttons for face registration and starting surveillance, making it intuitive for users.

## File Structure

```
face-surveillance-system/
├── main.py                # Main application script
├── yolov8n.pt             # YOLO model weights (downloaded)
├── README.md              # Project documentation
└── requirements.txt       # Python dependencies
```

## Code Workflow

1. **Load YOLO Model**: The YOLO model is loaded using PyTorch with GPU support (if available).
2. **Face Registration**: Captures face encodings and associates them with user-provided names.
3. **Motion Detection**: Identifies significant motion to trigger surveillance.
4. **Object and Face Detection**: Draws bounding boxes and labels on detected objects and recognized faces.
5. **GUI Interaction**: Provides easy-to-use buttons for registration and surveillance control.


## Use Cases

- Security monitoring in offices and homes.
- Intruder detection and alert systems.
- Surveillance systems for real-time tracking of individuals and objects.

## Future Enhancements

- Add email or SMS alerts for unknown or suspicious individuals.
- Integrate a database to store face encodings and logs.
- Support for multiple camera feeds.

## Acknowledgments

- [Ultralytics YOLO](https://github.com/ultralytics/ultralytics)
- [Face Recognition](https://github.com/ageitgey/face_recognition)

