# 🚗 Car_counter 
This projects demonstrates a car counting system using object detection techniques with YOLOv8. Thw system counts the number of cars passing through a designated area in a video. it employs object tracking to ensure accurate counting by tracking vehicles across frames.

---

## ✨ Features

- **Real-time object detection:** Detects cars in video frames using YOLOv8.
- **Car tracking:** Tracks vehicles across frames using a tracking algorithm.
- **Counting cars:** Displays the total number of cars passing by a specific region.
- **Customizable:** Easily adaptable to different videos and detection requirements.

---

## 📂 Project Structure

The project contains the following files:

1. **`main.py`:**
   - Core script for car detection and counting.
   - Implements the YOLOv8 model for object detection.
   - Displays the car count on the output video.
   
2. **`sort.py`:**
   - Tracks objects (cars) across frames to avoid duplicate counting.
   - This file was adapted from an external source to integrate a robust tracking mechanism.

3. **`graphics.png`:**
   - An image asset used for graphical elements in the project (e.g., overlays, UI enhancements).

4. **`mask.png`:**
   - A masking image used to define the area of interest for detecting and counting cars.

---

## Requirements

To run the project, install the following dependencies:

- Python 3.8 or higher
- Required Python libraries:
  ```bash
  pip install ultralytics opencv-python numpy
  ```

---

## Usage

1. Clone the repository or download the project files.
   ```bash
   git clone <repository-url>
   cd CarCounter
   ```

2. Place your input video in the project folder.

3. Run the `main.py` script:
   ```bash
   python main.py
   ```
   This script will process the video, detect cars, track them, and display the output video with the car count.

---

##🎥  How It Works

1. **Object Detection:**  
   YOLOv8 is used to detect cars in each frame of the video.

2. **Object Tracking:**  
   The `sort.py` file implements a tracking algorithm to assign unique IDs to detected cars and track them across frames.

3. **Counting Cars:**  
   The script determines when a car crosses a defined line or region and updates the count.

---

## Example Output

- **Input Video:** A sample video of vehicles moving along a road.![Car Counting Demo](car.gif) 
- **Output Video:** A video with detected cars highlighted and a real-time car count displayed.![Car Counting Demo](demo.gif) 

---

##🙏 Acknowledgments

- **SORT Algorithm:** The `sort.py` file is adapted from an external implementation to provide robust object tracking.

---

Let me know if you'd like to modify this further!
