# PythonPhoto

**PythonPhoto** is a Python library for capturing screenshots and processing images.
It supports Python 3.8–3.12 and provides an easy way to capture, edit, and save images directly from your desktop.

---

## Features

- Capture the **full screen** or a selected region.
- Save screenshots in **JPEG or PNG** formats.
- Basic **image processing** (resize, rotate, etc.).
- Easy integration with Python projects.

---

## Installation

```bash
git clone https://github.com/istoriya-islama/PythonPhoto.git
cd PythonPhoto
pip install -r requirements.txt
```

---

## Usage Examples

### 1. Capture full screen

```python
from PythonPhoto import PythonPhoto

# Capture full screen and save
PythonPhoto.capture_fullscreen("screenshot_full.png")
```

![Full screen example](sc/sc1.png)

---

### 2. Capture a selected region

```python
from PythonPhoto import PythonPhoto

# Capture a specific region (x, y, width, height)
PythonPhoto.capture_region(100, 100, 400, 300, "screenshot_region.png")
```

![Region capture example](sc/sc2.png)

---

### 3. Capture video frame

```python
from PythonPhoto import PythonPhoto

# Capture a video frame
PythonPhoto.capture_video_frame("video.mp4", "frame.png", 10) # 10th second
```

![Video frame example](sc/sc3.png)

---

### 4. Remove image or temporary file

```python
from PythonPhoto import PythonPhoto

# Remove an image
PythonPhoto.remove_image("screenshot_full.png")
```

![Remove image example](sc/sc4.png)

---

## Requirements

- Python 3.8–3.12  
- Pillow  
- OpenCV (`opencv-python`)  
- PyAutoGUI  
- PyScreenshot  
- NumPy  

---

## License

This project is licensed under the **GNU General Public License v3.0 (GPL-3.0)**.  
You are free to **use, modify, and distribute** this library under the terms of the license.

For more details, see the [GNU GPL v3.0](https://www.gnu.org/licenses/gpl-3.0.html).
