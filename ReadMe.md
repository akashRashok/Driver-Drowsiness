# Drowsiness Detection System

This project is a real-time drowsiness detection system that uses computer vision techniques to monitor a user's blink rate and eye closure. It triggers an alarm if it detects that the user's eyes have been closed for a concerning duration, indicating potential drowsiness. This is particularly useful for drivers or individuals in critical roles requiring high alertness.

## Features

- **Real-time Eye Tracking**: Monitors the user's eyes using a webcam and detects eye closure using the eye aspect ratio (EAR).
- **Drowsiness Alarm**: Triggers an audible alert when prolonged eye closure is detected, which could indicate drowsiness.
- **Facial Landmark Detection**: Utilizes Dlib's facial landmark detector to precisely locate and track the eyes.

## Dependencies

To run this project, you need the following libraries:

- `numpy`
- `dlib`
- `opencv-python`
- `imutils`
- `pyglet` (for audio playback)

Ensure you have Python installed on your system. This project was developed using Python 3.x.

## Installation

1. Clone the repository
2. Install the required packages:
- pip install numpy dlib opencv-python imutils pyglet
3. Download the dat file from the link provided below to run the program
- https://drive.google.com/drive/folders/1rkIvWjdHQjB0lEx-Mbyg9whPil2Zf1lV?usp=sharing

## Usage

To start the drowsiness detection, simply run the script from the command line

## How It Works

The system uses a pre-trained facial landmark detector from Dlib to find the facial landmarks. It calculates the EAR for both eyes and if the EAR falls below a threshold for a specified number of consecutive frames, it triggers an alarm sound.

## Configuration

- **EYE_AR_THRESH**: The threshold value for the eye aspect ratio below which the alarm is triggered.
- **EYE_AR_CONSEC_FRAMES**: The number of consecutive frames the EAR must be below the threshold to consider the user as drowsy.

## Contributing

Feel free to fork the repository and submit pull requests. You can also open an issue for bugs, suggestions, or comments.

## Acknowledgments

- Thanks to the Dlib library and its contributors for providing the facial landmark detection model.
