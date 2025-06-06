# Forest Fire Identification Using UAV Video Monitoring

This project implements a **forest fire detection system** using **motion detection**, **color feature analysis**, and **video input from UAVs (Unmanned Aerial Vehicles)**. The application is built with Python and uses the **OpenCV** and **Tkinter** libraries to create a GUI for analyzing forest fire videos.

---

## 🧠 Project Summary

Forest fires are a major environmental concern, and early detection is crucial. This system helps identify possible fire occurrences in video footage captured by UAVs. It analyzes motion and color features (in HSV space) and displays alerts when fire is detected in the frame.

---

## 💻 Features

- GUI-based application using Tkinter
- Upload UAV video footage (`.mp4`, `.avi`, etc.)
- Real-time video processing with:
  - Color feature detection (fire-like color ranges in HSV)
  - Motion detection (frame differencing)
- Fire alert displayed on video
- Optional contour drawing (currently commented out)

---

## 🔧 Tech Stack

- **Language:** Python 3.x
- **Libraries:**
  - `OpenCV` – for image processing and video analysis
  - `Tkinter` – for GUI development
  - `NumPy` – for numerical operations
  - `cv2` – for OpenCV functionality
    
---Detection Techniques
Color Detection in HSV Space:

Fire-like colors fall within HSV range [18, 50, 50] to [35, 255, 255].

If detected pixels > 4000 → "Fire Detected" is shown.

Motion Detection:

Frame differencing and thresholding is used.

Detects significant pixel movement between consecutive frames.

(Optional) Wavelet Transform/Contour Detection:

Code is ready but commented out; can be used to draw bounding boxes on fire regions.

---Future Improvements
Add deep learning-based fire classification (e.g., CNNs)

Add logging for detected fire timeframes

Export fire-flagged frames for offline review

Implement wavelet transform or thermal imaging integration

