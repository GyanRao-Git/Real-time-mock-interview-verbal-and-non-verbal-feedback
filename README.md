# 🎯 Real-Time Mock Interview Feedback System

This project tackles the challenge of providing **real-time feedback during mock interviews** by analyzing **verbal and non-verbal cues** through emotion recognition. We developed an intelligent system that evaluates **facial expressions**, **vocal tone**, and **spoken content** to simulate human-like feedback for interviewees.

---

## 🧠 What We Built

We explored **three core modalities**, each using a dedicated model:

### 👁️ Visual Modality
A **ResNet18** model trained on the **AffectNet** dataset to classify facial emotions.  
✅ **Achieved 69% accuracy**

### 🔊 Audio Modality
A **Random Forest** classifier trained on **RAVDESS** audio samples using MFCC features to detect speech-based emotions.  
✅ **Achieved 63.9% accuracy**

### 🗣️ Text Modality
A **lightweight NLP model** using **MediaSum** data to assess summary quality in terms of **sentiment**, **keyword coverage**, and **fluency**.  
✅ **Achieved 77% accuracy**

---

## 🔀 Multimodal Fusion (What Didn't Work)

We also attempted to combine the above signals into a **multimodal fusion model**. Unfortunately, this approach underperformed:

❌ **Multimodal Accuracy: 18.5%**

### 📉 Why It Failed:
- 🔄 **Asynchronous inputs** across modalities  
- ⏱️ **Lack of temporal alignment or modeling**  
- 📉 **Noisy fusion techniques** without end-to-end optimization

---

## 💡 Key Takeaways

- ✅ **Unimodal models are more robust** for real-time mock interview settings
- 🧩 **Facial emotion recognition** provides insight into confidence and engagement
- 🎤 **Audio emotion analysis** reflects tone, stress, and emotional state
- 📝 **Text-based feedback** can assess the clarity and sentiment of verbal responses
