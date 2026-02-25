Acess the file here:- https://colab.research.google.com/drive/1aGl4Bv_C64bEdDLtn8QrAdUllHuoacQN?usp=sharing

# 🌿 LeafRx

## A Deep Learning-Based Multi-Class Plant Disease Diagnosis and Treatment Recommendation System

---

## 📌 Overview

**LeafRx** is an end-to-end intelligent crop health diagnostic system that combines deep learning–based computer vision with an integrated treatment recommendation engine to detect and manage plant diseases.

The system classifies plant leaf images into **39 distinct categories** (healthy and diseased) across multiple crop types and provides actionable pesticide or management recommendations based on the predicted condition.

LeafRx moves beyond simple image classification — it functions as a digital plant health assistant capable of assisting farmers in early disease detection, preventive care, and informed agricultural decision-making.

---

## 🌍 Problem Statement

Plant diseases are responsible for billions of dollars in annual crop losses worldwide. Traditional disease identification methods:

* Require domain expertise
* Are time-consuming
* Are often inaccessible in rural areas
* Delay intervention, increasing yield loss

Small and marginal farmers are especially vulnerable due to limited access to agronomists and laboratory diagnostics.

LeafRx addresses this gap by offering:

* Rapid diagnosis from leaf images
* AI-driven classification
* Immediate treatment guidance
* Scalable, low-cost deployment potential

---

## 🧠 System Architecture

LeafRx follows a structured AI pipeline:

```
Image Upload
      ↓
Image Preprocessing (160x160, normalization)
      ↓
EfficientNet-Based CNN Model
      ↓
Multi-Class Disease Prediction (39 classes)
      ↓
Disease-Type Identification (Fungal / Bacterial / Viral / Pest)
      ↓
Treatment Recommendation Engine
      ↓
Human-Readable Advisory Report
```

---

## 🔬 Technical Implementation

### 📊 Dataset

* 39 plant disease classes
* Publicly available dataset from Mendeley Data
* Augmented dataset for improved generalization
* Train: 80%
* Validation: 10%
* Test: 10%

### 🖼 Preprocessing

* Image resizing to 160×160
* Batch size: 32
* Data shuffling and augmentation
* EfficientNet preprocessing pipeline

### 🧠 Model Architecture

* Backbone: **EfficientNet (Transfer Learning)**
* Pretrained on ImageNet
* Frozen base layers (initial phase)
* Fine-tuning of deeper layers
* Classification Head:

  * Global Average Pooling
  * Dropout (0.2)
  * Dense layer (39 outputs, softmax)

### 📈 Performance

* Validation Accuracy: ~94.6%
* Test Accuracy: ~96.44%
* Low validation loss (~0.08)
* Strong generalization
* Minimal overfitting observed

---

## 💊 Intelligent Treatment Recommendation System

Unlike conventional classification-only systems, LeafRx integrates a rule-based advisory module.

Each predicted disease is mapped to:

* Disease type (Fungal / Bacterial / Viral / Pest)
* Suggested pesticide or control measure
* Application guidance
* Preventive recommendations

For viral infections (e.g., Tomato Mosaic Virus), where no direct chemical cure exists, the system recommends containment strategies and vector control.

This makes LeafRx a **decision-support tool**, not just a classifier.

---

## 🌾 Impact on Farmers

LeafRx has significant potential to transform agricultural disease management:

### 1️⃣ Early Detection

Timely identification reduces disease spread and crop damage.

### 2️⃣ Reduced Crop Loss

Early intervention can significantly reduce yield loss, especially in high-value crops like tomato, grape, and apple.

### 3️⃣ Lower Dependency on Experts

Farmers in remote areas can access AI-driven guidance without waiting for agronomists.

### 4️⃣ Optimized Pesticide Usage

By recommending targeted treatments:

* Reduces overuse of chemicals
* Minimizes environmental impact
* Lowers input costs

### 5️⃣ Food Security Enhancement

Improved disease management leads to:

* Higher crop yield
* Better quality produce
* Reduced economic vulnerability

---

## 🌱 Sustainability Benefits

LeafRx promotes sustainable agriculture by:

* Encouraging precision pesticide application
* Reducing blanket spraying practices
* Supporting disease-specific treatment
* Potential integration with organic alternatives in future versions

With proper expansion, this system could support climate-resilient farming practices.

---

## 📱 Deployment Potential

LeafRx is designed to be:

* Deployable as a web application
* Integrated into mobile applications
* Adaptable for edge devices
* Usable in low-resource environments

The trained model can be exported and deployed via:

* TensorFlow Lite
* REST APIs
* Streamlit or Flask-based applications

---

## 🔮 Future Scope

* Severity estimation module
* Multi-language support for farmers
* Real-time camera integration
* Region-specific pesticide regulation filtering
* LLM-powered conversational advisory system
* Integration with satellite or IoT crop monitoring

---

## 📚 Research Significance

LeafRx demonstrates:

* The effectiveness of transfer learning in agricultural AI
* Practical integration of CNN models with advisory systems
* High accuracy with moderate computational requirements
* Scalability for precision agriculture applications

It serves as a foundation for future research in:

* AI-driven agronomy
* Sustainable farming technologies
* Automated crop surveillance systems
* Multimodal agricultural intelligence systems

---

## 🧑‍💻 Author

**Shivam Nichit**
B.Tech Bioinformatics & Data Science
DY Patil University

---
