# 🖼️ **Transfer Learning for Image Classification**  
### 🔬 **By Alankrutha Reddy Purumandla**  

---

## 🎯 **Project Overview**
This project explores **Transfer Learning** for image classification by focusing on two commonly confused objects: **smartphones** and **remote controls**. Using pre-trained models, we aim to demonstrate how transfer learning can handle **data scarcity** while maintaining high classification accuracy.  

Key Models:  
- 🏆 **VGG16**  
- 🔄 **ResNet50**  
- 📱 **MobileNet**  
- ⚡ **EfficientNet**

---

## 📖 **Abstract**  
This research investigates:
1. The **efficiency** of transfer learning in image classification.  
2. The **minimum training data size** needed to achieve 90% accuracy.  
3. The **trade-off** between accuracy and computational efficiency.

We created a custom dataset of smartphone and remote control images with diverse orientations and applied transfer learning strategies such as feature extraction and fine-tuning.

---

## 🌟 **Features**
- **Custom Dataset**: Curated images of smartphones and remote controls.
- **Pre-Trained Models**: Leveraged models like VGG16 and MobileNet.  
- **Data Augmentation**: Techniques like rotation, scaling, and flipping to enhance robustness.
- **Performance Insights**: Comparative evaluation of models with varying training sizes.

---

## 🛠️ **Technologies Used**
| **Category**       | **Tools/Libraries**         |
|---------------------|-----------------------------|
| Programming Language | Python 3.8                |
| ML Framework        | TensorFlow/Keras           |
| Dataset Curation    | BeautifulSoup, Requests    |
| Visualization       | Pillow, Matplotlib         |

---

## 🔬 **Methodology**
### **1. Dataset Creation**  
- Collected images from:  
  - 📂 **Google Open Images Dataset**  
  - 🌐 **Wikimedia Commons**  
  - 🖼️ **Public Domain Pictures**  
- Preprocessed images to ensure uniformity and augmented data to improve model performance.  

### **2. Transfer Learning Workflow**  
- Utilized the **convolutional base** of pre-trained models with frozen weights.  
- Added fully connected layers with **ReLU activation** and **Dropout** regularization.  
- Used a **Sigmoid activation function** for binary classification.  

### **3. Training and Evaluation**  
- Split data into training and validation sets.  
- Evaluated models on varying training sizes from **20** to **1200 samples**.  
- Recorded validation accuracy and training time.  

---

## 📊 **Results**
### **Validation Accuracy Comparison**  
| **Model**         | **Training Samples** | **Accuracy** |
|--------------------|----------------------|--------------|
| VGG16             | 500                  | 90%          |
| MobileNet         | 1000                 | 90%          |
| ResNet50          | 1200                | 88%          |
| EfficientNet      | 1200                | 75%          |

### **Training Time**  
| **Model**         | **Training Samples** | **Time (Seconds)** |
|--------------------|----------------------|--------------------|
| VGG16             | 500                  | 709                |
| MobileNet         | 1000                 | 235                |
| ResNet50          | 1200                 | 489                |
| EfficientNet      | 1200                 | 554                |

### **Insights**
- 🏆 **VGG16**: Achieved 90% accuracy fastest with 500 samples.  
- ⚡ **MobileNet**: Most computationally efficient, training in just 235 seconds for 1000 samples.  
- 🔄 **ResNet50**: Consistent performance but required more data to achieve high accuracy.  
- ⚠️ **EfficientNet**: Struggled with data variability, showing high fluctuations in accuracy.

---

🚀 How to Run
1. Clone the repository
git clone https://github.com/Alankrutha18/Transfer-Learning-Image-Classification.git

2. Install dependencies:
pip install tensorflow beautifulsoup4 pillow matplotlib

3. Run the training script:
python scripts/train_model.py

----

📌 Future Work
Extend the project to multi-class classification.
Explore additional pre-trained models like InceptionV3.
Evaluate real-time applications on resource-constrained devices.


