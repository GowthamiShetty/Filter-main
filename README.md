# Webcam Filter Application

This project is a simple webcam-based application that applies various fun filters to detected faces in real-time, similar to Snapchat filters. The application allows users to switch between different filters, capture images, and record videos with the applied filters.

## Features

- *Real-time Face Detection*: Uses Haar Cascades to detect faces in the video feed.
- *Filter Overlays*: Applies different overlays (filters) to detected faces.
- *Image Capture*: Allows capturing and saving images with the applied filters.
- *Video Recording*: Allows starting and stopping video recording with the applied filters.

## Requirements

- Python 3.x
- OpenCV
- cvzone
- Pillow (PIL)

## Installation

1. Clone the repository:
    bash
    git clone https://github.com/GowthamiShetty/webcam-filter-app.git
    cd webcam-filter-app
    

2. Install the required Python packages:
    bash
    pip install opencv-python opencv-python-headless cvzone pillow numpy
    

3. Make sure you have the overlay images (cool.png, beard.png, sunglass.png, native.png, pirate.png) in the project directory.

Key Controls
q: Quit the application.
n: Switch to the next filter.
p: Switch to the previous filter.
c: Capture and save the current frame as an image.
r: Start/Stop video recording.

Code Explanation
The main steps of the code are as follows:

Import Libraries: Import necessary libraries including OpenCV, cvzone, PIL, and numpy.

Initialization: Initialize the webcam, face detection classifier, and load overlay images.

Video Capture and Processing Loop: Continuously capture frames from the webcam, detect faces, apply filters, and handle user inputs.

Face Detection: Convert the frame to grayscale and detect faces using Haar Cascades.

Apply Filters: Resize and apply the current filter to detected faces.

Display Frame: Display the processed frame with overlays.

Handle Key Presses: Allow users to switch filters, capture images, and start/stop video recording.

Video Recording: Write frames to a video file when recording is active.

Cleanup: Release resources and close windows when done.

Example Overlays
Ensure you have these example overlays in your project directory:
cool.png
beard.png
sunglass.png
native.png
pirate.png
Feel free to add more overlays by simply placing the image files in the project directory and updating the overlay_paths list in the code.

Contributing
Contributions are welcome! Please feel free to submit a Pull Request.

Contact
For any inquiries or feedback, please contact [shettygowthami80@gmail.com].
