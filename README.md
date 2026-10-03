# 🏋️ Virtual Coach – AI-Powered Fitness Coach Using Computer Vision 🚀
 
### 📌 Project Overview
 
**Virtual Coach** is an AI-powered fitness coach that analyzes an athlete's movements from video recordings and compares them with reference movements.
 
The project uses **Keypoint R-CNN** to detect human body keypoints and evaluate exercise execution quality through pose similarity analysis.
 
💡 **Use Cases:**
✅ Fitness training (squats, push-ups, planks)
✅ Dance and sports movement analysis
✅ Martial arts technique assessment
✅ Fitness gamification 🎮
 
---
 
## 📂 Project Structure
 
```text
VirtualCoach/
├── src/
│ ├── keypoint_detector.py
│ ├── procrustes_analysis.py
│ ├── similarity_metrics.py
│ ├── process_video.py
│ ├── visualization.py
│ └── main.py
├── images/
├── examples/
├── scripts/
│ ├── train.py
│ ├── evaluate.py
│ └── run_analysis.py
├── README.md
├── requirements.txt
└── LICENSE
```
 
---
 
## 🎥 How Virtual Coach Works
 
📌 **1. Load an athlete's video and a reference video**
 
📌 **2. Extract video frames**
 
📌 **3. Detect body keypoints using Keypoint R-CNN**
 
📌 **4. Apply Procrustes alignment for pose normalization**
 
📌 **5. Compare movements using similarity metrics:**
- Cosine similarity (pose angle analysis)
- Weighted matching (keypoint confidence evaluation)
 
📌 **6. Visualize differences and generate exercise quality scores**
 
---
 
## 📊 Results
 
| Metric | Value |
|----------|----------|
| Average Cosine Similarity | **0.9828** |
| Average Weighted Match Score | **59.1997** |
 
📌 **Higher values indicate better alignment between the performed exercise and the reference movement.**
 
---
 
## 🚀 How to Run the Project
 
### 🔧 Install Dependencies
 
```bash
git clone https://github.com/Alex1988Den/VirtualCoach.git
cd VirtualCoach
pip install -r requirements.txt
```
 
### 🎥 Run Video Analysis
 
```bash
python src/main.py --reference "path_to_ref_video.mp4" --input "path_to_user_video.mp4"
```
 
---
 
## 🛠 Technologies
 
- Python
- PyTorch
- Torchvision
- OpenCV
- Matplotlib
- NumPy
- SciPy
 
---
 
## 👨‍💻 Author
 
Developed by **Aleksandr Denissov**
 
If you find this project useful, feel free to leave a ⭐ on GitHub.
