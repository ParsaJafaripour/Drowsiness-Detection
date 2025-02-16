# Drowsiness Detection

A real-time drowsiness detection application built in Python using a custom-trained YOLOv5 model. This project utilizes PyTorch for deep learning inference, OpenCV for video processing, and Tkinter/CustomTkinter for the graphical user interface.

## Features

- **Real-Time Video Processing:** Captures live webcam feed and processes each frame.
- **Deep Learning Integration:** Uses a custom-trained YOLOv5 model to detect signs of drowsiness.
- **User Interface:** Displays live video with detections, a counter for drowsiness events, and a reset button.
- **Easy to Use:** Simply run the application, and the GUI will handle the rest.

## How It Works

1. **Video Capture:** The app captures the webcam feed using OpenCV.
2. **Detection:** Each frame is converted to RGB and passed through the YOLOv5 model to identify drowsiness events.
3. **Counter Update:** If the model detects drowsiness with high confidence (over 85%), a counter increments.
4. **GUI Display:** The live video and current count are displayed in a user-friendly window built with Tkinter and CustomTkinter.

## Installation

1. **Clone the Repository:**
   ```bash
   git clone https://github.com/yourusername/Drowsiness-Detection.git
   cd Drowsiness-Detection
   ```

2. **Create and Activate a Virtual Environment:**
   ```bash
   python -m venv venv
   # Activate on Windows (CMD)
   venv\Scripts\activate
   # Or on macOS/Linux:
   source venv/bin/activate
   ```

3. **Install Dependencies:**
   ```bash
   pip install -r requirements.txt
   ```
   *(Make sure your `requirements.txt` includes packages like `torch`, `opencv-python`, `customtkinter`, `Pillow`, and `numpy`.)*

4. **Download the Custom YOLOv5 Weights:**  
   Update the path in the code to point to your custom weights file.

## Usage

Run the application:
```bash
python app.py
```
A window will open displaying the live video feed with detections. The counter will increment for each drowsiness event detected, and you can reset the counter using the provided button.
