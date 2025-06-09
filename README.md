# Object Tracking

This project demonstrates a basic but effective approach to **object detection** and **tracking** using OpenCV. It focuses on identifying and tracking vehicles on a highway using a fixed surveillance camera. The technique combines background subtraction, noise filtering, and tracking with unique IDs to count and follow objects frame by frame.

---

## Project Structure
```
object_tracking/
├── main.py # Main file to run object detection and tracking
├── tracker.py # Contains the tracking class logic
└── highway.mp4 # Input video of a highway for vehicle tracking
```

---

## Overview

### Object Detection
- Detects motion using `cv2.createBackgroundSubtractorMOG2()`.
- Filters out noise using contour area thresholding.
- Focuses only on a **Region of Interest (ROI)** to improve performance and accuracy.

### Object Tracking
- Tracks objects using a simple **Euclidean Distance Tracker** implemented in `tracker.py`.
- Each detected object is assigned a **unique ID**.
- Tracks position frame-by-frame and draws bounding boxes with IDs.

---

## Requirements

- Python 3.x
- OpenCV: `pip install opencv-python`

---

## Setup Instructions
1. **Clone the Repository**

   ```
   git clone https://github.com/Deadshot994/Object-Tracking.git
   ```

## License
This project is open-source and available under the [MIT License](LICENSE).

## Author
Sanjeeth Manikandan