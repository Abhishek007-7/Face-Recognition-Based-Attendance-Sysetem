# Face-Recognition-Based-Attendance-Sysetem
 Engineered a Python-based attendance system incorporating advanced facial recognition  algorithms, ensuring precise identification; enhanced reliability for various applications and  decreased human error in attendance logging.


```markdown
# Face Recognition-Based Attendance System

## Overview

The Face Recognition-Based Attendance System is a Python application that utilizes OpenCV and Dlib for real-time face detection and recognition. The application captures images from a webcam and allows users to register their faces. The registered faces are stored in a structured format for later use in attendance tracking.

## Features

- Real-time face detection using Dlib.
- User-friendly interface built with Tkinter.
- Save registered faces to a designated folder.
- Log messages and status updates in the GUI.
- Integration with an SQLite database to save attendance records.

## Prerequisites

Before running the application, ensure you have the following installed:

- Python 3.x
- Required libraries:
  - OpenCV
  - Dlib
  - NumPy
  - Tkinter
  - Pillow

You can install the required libraries using pip:

```bash
pip install opencv-python dlib numpy pillow
```

## Project Structure

```
├── data
│   ├── data_faces_from_camera
│   └── features_all.csv
├── attendance.db
├── get_faces_from_camera_tkinter.py
└── README.md
```

- **data/**: Directory for saving registered face images and features.
- **attendance.db**: SQLite database file for storing attendance records.
- **get_faces_from_camera_tkinter.py**: Main Python script for the face recognition system.
- **README.md**: Documentation file for the project.

## How to Use

1. **Clone the Repository**:

   ```bash
   git clone <repository-url>
   cd <repository-folder>
   ```

2. **Run the Application**:

   Execute the main script:

   ```bash
   python get_faces_from_camera_tkinter.py
   ```

3. **Register Faces**:

   - Input your name in the provided field and click "Input" to create a folder for saving your face images.
   - Ensure your face is visible on the webcam, and click "Save current face" to capture and save your face image.

4. **Attendance Tracking**:

   - The attendance will be saved automatically to the `attendance.db` database when a recognized face is detected.

5. **Clear Old Data**:

   - Click on "Clear" to delete old registered face images and reset the system.

## Logging

The application logs messages to the console, including status updates on face registration and saving.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Acknowledgments

- [Dlib](http://dlib.net/) for the face detection library.
- [OpenCV](https://opencv.org/) for image processing functionalities.
- [Tkinter](https://docs.python.org/3/library/tkinter.html) for the GUI.

## Author

- **Abhishek** 
