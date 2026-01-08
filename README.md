### 🌿🌳 CNN-Based Plant Health Detection System
A deep learning–based plant health monitoring system that uses Convolutional Neural Networks (CNNs) to detect diseases and stress conditions from both plant leaves and tree trunks.<br>
Built with TensorFlow & Keras, the system aims to support early disease detection in agriculture and forestry.

---

### 🚀 Project Overview
Plant diseases often appear on leaves (spots, discoloration, texture changes) as well as tree trunks (fungal growth, cracks, bark decay).
This project extends traditional leaf-based classification by supporting multi-surface plant analysis, making it suitable for real-world agricultural and forestry applications.

---

### ✅ What This Model Can Detect
- Healthy vs diseased leaves
- Visible disease/stress patterns on tree trunks
- Multiple disease classes using image-based classification

---

### 🧠 Why CNNs?
- Convolutional Neural Networks are ideal for this task because they:
- Automatically extract visual features (texture, edges, patterns)
- Work well on complex biological images
- Scale efficiently for multiple disease categories
- Reduce dependency on manual feature engineering

---

### 🖥️ Hardware Requirements & GPU Support

This project supports both CPU and GPU execution. GPU acceleration is highly recommended for faster training and experimentation.

#### ✅ Minimum Hardware Requirements (CPU)
| Component | Requirement |
|---------|------------|
| CPU     | Intel i5 / Ryzen 5 or equivalent |
| RAM     | 8 GB (16 GB recommended) |
| Storage | 5–10 GB free space |
| OS      | Windows / Linux / macOS |
| Python  | 3.8 – 3.10 |


#### 🚀 Recommended Hardware (GPU)
| Component | Requirement |
|---------|------------|
| GPU     | NVIDIA GPU with ≥ 4 GB VRAM |
| CUDA    | 11.2 (Compatible with TensorFlow 2.10) |
| cuDNN   | 8.1 (Matching CUDA version) |
| RAM     | At least 8 GB |
| Storage | SSD recommended |

---

### 🛠️ Technologies Used & Why
**Core Deep Learning**
- **TensorFlow 2.10.0** - Provides a stable and production-ready framework for building and training CNN models.
- **Keras 2.10.0** - Simplifies neural network design and integrates seamlessly with TensorFlow.
  
**Model Optimization**
- **Keras-Tuner 1.4.8** - Used to tune CNN hyperparameters (filters, learning rate, kernel size) to improve classification accuracy.

**Image Processing**
- **Pillow 12.0.0** - Used for loading, resizing, and preprocessing leaf and trunk images.
  
**Data Handling & Computation**
- **NumPy 1.23.5** – Efficient numerical operations
- **SciPy 1.15.3** – Scientific computing support
- **Pandas 2.3.3** – Label handling and dataset management

**Evaluation & Visualization**
- **scikit-learn** – Metrics, data splitting, evaluation
- **matplotlib** – Training & validation graphs
- **seaborn** – Confusion matrices and heatmaps

#### 📦 Installation Requirements
✅ Supported Python Version - Python 3.8 – 3.10

#### 📥 Install Dependencies
```
pip install -r requirements.txt
``` 

---

### 📂 Project Structure
```
CNN-Plant-Health-Detection-Model/
├── Utils/
│   └── ImgNameChanger.py        # Dataset preprocessing utility
├── health_classifier/           # Dataset of images
├── keras_tuner_dir/             # Hyperparameter tuning logs
├── class_labels_combined.json   # Leaf & trunk class mappings
├── plantDiseaseDetection.ipynb  # Training, evaluation & prediction
├── requirements.txt             # Dependencies
├── .gitignore
└── README.md
```

---

### 🗂️ Dataset Directory Structure
Organize your dataset as follows:
```
health_classifier/
├── train/
│   ├── healthy/
│   └── diseased/
├── val/
│   ├── healthy/
│   └── diseased/
```
#### 📌 Important:
healthy/ contains both healthy leaves and healthy trunks

diseased/ contains both diseased leaves and diseased trunks

---

### 📸 Image Collection Guidelines
#### Healthy Class
Include:
- Healthy leaves (normal color, no spots)
- Healthy trunks (intact bark, no fungal growth)

#### Diseased Class
Include:
- Diseased leaves (spots, blight, curling, discoloration)
- Diseased trunks (fungal growth, cracks, decay)

#### ✅ Best Practices
- Use different lighting conditions
- Capture multiple angles
- Avoid blurry images
- Minimum image size: 224 × 224

#### 🧹 Data Cleaning & Quality Control
##### Before training:
- Remove duplicate images
- Remove corrupted or unreadable files
- Ensure correct labeling (healthy vs diseased)
- Keep class balance as close as possible
##### Recommended: 500+ images per class for better generalization

#### 🛠️ Dataset Preprocessing
##### The training pipeline automatically handles:
- Image resizing
- Pixel normalization
- Label encoding (healthy = 0, diseased = 1)
- Training & validation splitting
##### Optional utility: Utils/ImgNameChanger.py - for renaming images consistently.

#### 📈 Improving Dataset Performance
##### You can improve results by:
- Adding more trunk images (often underrepresented)
- Using data augmentation (rotation, flip, zoom)
- Including early-stage disease samples
- Mixing field and lab images

#### ⚠️ Common Dataset Mistakes
- Mixing healthy and diseased images
- Highly imbalanced classes
- Poor lighting or low resolution
- Wrong folder names

#### ✅ Why This Dataset Design Works
- Simple binary classification
- Faster training
- Real-world applicability
- Easier deployment
- Supports both leaves and trunks naturally

---

### 🧪 How It Works
**Image Input**
- Leaf images (spots, discoloration, curling)
- Trunk images (bark damage, fungal growth, decay)

**Preprocessing**
- Image resizing & normalization
- Label encoding
- Dataset splitting (train/validation)

**CNN Training**
- Feature extraction using convolution layers
- Classification using dense layers

**Prediction**
- Outputs disease class
- Provides prediction confidence score

---

### 📊 Key Features
- Leaf and trunk disease detection
- CNN-based deep learning model
- Hyperparameter tuning support
- Modular & scalable ML design
- Ready for API & deployment integration

---

### 👤 Author
Titash Majumder<br>
B.Tech – Information Technology<br>
RCC Institute Of Information Technology<br>
Interests: Machine Learning, Python Development, Cybersecurity<br>
🔗 GitHub: https://github.com/TitashMajumder<br>
🔗 LinkedIn: https://www.linkedin.com/in/titash-majumder-38a6261b6/

---

### 📜 License
This project is open-source and intended for educational and research purposes.
