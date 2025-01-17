
# Helmet and Face Detection Using YOLOv5

This repository demonstrates the use of YOLOv5 for object detection, specifically for detecting helmets and faces. The project includes pre-trained custom models and test images to evaluate the detection performance in noisy environments.

---

## **Repository Structure**

```
Helmet-and-Face-Detection-YOLO/
├── yolo-helmets.pt         # Pre-trained YOLOv5 model for helmet detection
├── yolo-faces.pt           # Pre-trained YOLOv5 model for face detection
├── noisy test images/      # Folder containing noisy test images
├── Helmet_and_Face_Detection.ipynb  # Python notebook for object detection
├── detect_helmets_faces.py # Script version of the notebook
└── README.md               # Project documentation
```

---

## **Features**
- Detect helmets and faces in images using YOLOv5.
- Visualize bounding boxes and labels on the detected objects.
- Filter detections to focus on specific classes (e.g., helmets or faces).
- Resize and display the processed images for quick evaluation.

---

## **Applications**
This project is particularly useful for safety monitoring in industrial environments where wearing helmets is mandatory. It can help:
- Ensure compliance with safety regulations.
- Monitor workers for proper use of personal protective equipment (PPE).
- Enhance workplace safety by identifying individuals without helmets.

---

## **Getting Started**

### **Prerequisites**
Ensure you have the following installed:
- Python 3.8+
- OpenCV
- PyTorch

Install the required Python libraries:
```bash
pip install torch numpy opencv-python
```

### **Running the Project**
1. Clone the repository:
   ```bash
   git clone https://github.com/NouraMaklad/Helmet-and-Face-Detection-YOLO.git
   cd Helmet-and-Face-Detection-YOLO
   ```

2. Run the Python script:
   ```bash
   python detect_helmets_faces.py
   ```

3. Alternatively, open the Jupyter Notebook `Helmet_and_Face_Detection.ipynb` for an interactive experience.

---

## **How It Works**
1. **Model Loading**:
   - The `yolo-helmets.pt` model is used for helmet detection.
   - The `yolo-faces.pt` model is used for face detection.

2. **Detection Process**:
   - Images from the `noisy test images/` folder are processed.
   - YOLOv5 detects objects and draws bounding boxes and labels.

3. **Class Filtering**:
   - You can specify which classes to detect by modifying the `model.classes` parameter.

---

## **Example Outputs**
Processed images are displayed with bounding boxes and labels for detected helmets and faces, highlighting individuals who are compliant or non-compliant with helmet requirements.

---

## **Acknowledgements**
- [YOLOv5 by Ultralytics](https://github.com/ultralytics/yolov5) for the base detection framework.
