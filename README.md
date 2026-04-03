**🧍‍♂️ Multi-Pose Detection System**
=====================================

A real-time **multi-person pose detection system** that identifies and tracks multiple human body keypoints from video streams (webcam or video input). This project leverages deep learning-based pose estimation to visualize human skeletal structures dynamically.

**🚀 Overview**
---------------

This project performs **multi-pose detection**, which means it can:

*   Detect **multiple people simultaneously**
    
*   Extract **key body keypoints (joints)**
    
*   Draw **skeletal connections**
    
*   Process **real-time video streams**
    

Human pose estimation is a core computer vision task where body joints (like elbows, knees, etc.) are detected from images or video  .

**🧠 Features**
---------------

*   🎥 Real-time webcam pose detection
    
*   👥 Multi-person detection support
    
*   🔗 Skeleton visualization using keypoint connections
    
*   📊 Confidence-based keypoint filtering
    
*   ⚡ Optimized for performance (supports high-resolution inputs)
    

**🏗️ System Architecture**
---------------------------
Input Video / Webcam
        ↓
Frame Capture (OpenCV)
        ↓
Preprocessing (Resize / Normalize)
        ↓
Pose Estimation Model (e.g., MoveNet / DL Model)
        ↓
Keypoint Extraction (17 joints per person)
        ↓
Multi-person Loop Processing
        ↓
Skeleton Rendering
        ↓
Output Display


**🧪 Tech Stack**
-----------------

*   **Python**
    
*   **OpenCV**
    
*   **TensorFlow / TensorFlow Hub**
    
*   **NumPy**
    
*   **Matplotlib (optional)**


### **Requirements**
tensorflow
opencv-python
numpy
matplotlib
tensorflow-hub

### **Run with Webcam**
python main.py

### **Run with Video File**
python main.py --source path/to/video.mp4

**📊 How It Works**
-------------------

1.  Video frames are captured using OpenCV.
    
2.  A pretrained deep learning model detects human figures and predicts keypoints.
    
3.  Each person is assigned:
    
    *   17 keypoints (nose, shoulders, elbows, etc.)
        
    *   Confidence score per keypoint
        
4.  The system loops through all detected individuals and processes them independently.
    
5.  Keypoints are connected to form a skeleton structure.
    

Multi-person pose estimation typically involves detecting individuals first and then estimating pose per person (top-down approach)  .

**📷 Output**
-------------

*   Bounding boxes around detected persons
    
*   Keypoints plotted on joints
    
*   Lines connecting joints to form skeleton
    

**📈 Applications**
-------------------

*   🏋️ Fitness tracking
    
*   🎮 Gesture-based control
    
*   🎥 Surveillance & activity recognition
    
*   🤖 Human-computer interaction
    

Pose estimation is widely used in tracking, surveillance, and interaction systems  .
