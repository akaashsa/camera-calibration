# camera-calibration
# 🧠 Synthetic Camera Calibration and Distortion Demo

This project simulates a real-world camera calibration workflow using synthetic lens distortion on a chessboard image. It demonstrates how to:

- Apply simulated distortion to an ideal image using OpenCV
- Perform calibration using detected chessboard corners
- Recover the original camera parameters
- Undistort the distorted image using the recovered calibration
- Visually compare all stages

---


---

## 🧪 Methods Used

- `cv2.initUndistortRectifyMap` to simulate lens distortion
- `cv2.findChessboardCorners` for calibration pattern detection
- `cv2.calibrateCamera` to estimate camera intrinsics and distortion
- `cv2.undistort` for correcting distorted images
- `matplotlib` for visualizing Original → Distorted → Undistorted flow

---

## 📊 Outputs

You will see a 3-panel comparison:

1. **Original**: Clean input image (ideal camera)
2. **Distorted**: Simulated output from a distorted lens
3. **Recovered**: Corrected image using calibration recovery

---

## 🛠 Requirements

Install dependencies with:

```bash
pip install opencv-python numpy matplotlib
