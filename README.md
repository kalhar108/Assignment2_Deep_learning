# CMPE-258 Assignment 2 - Deep Learning (Spring 2026, Sec 49)

## 📋 Overview

This repository contains all four parts of Assignment 2 for CMPE-258 Deep Learning. Each part demonstrates different aspects of modern AI/ML development including multimodal AI, full-stack web development with AI, cross-platform mobile development, and neural network implementation.

## Youtube Links:
- 1) Part A: Multimodal AI with Google Gemini : https://youtu.be/dN8BPRK9Hzs
- 2) Part B: SpendWise AI - Smart Expense Tracker (Web App): https://youtu.be/oeBcCx95Hn4
- 3) Part C: MindFlow - AI Mood & Wellness Journal (Mobile App): https://youtu.be/ypGPd7VQGkY
- 4) Part D: MNIST Neural Network Classifier: https://youtu.be/vGT-1B31Bqc

---

## 📁 Repository Structure

```
assignment1/
├── README.md
├── partA/
│   └── CMPE258_Assignment1_PartA_Multimodal_AI.ipynb
├── partB/
│   ├── spendwise-web-app.html
│   └── README.md
├── partC/
│   ├── mindflow-mobile-app.html    (Interactive prototype)
│   ├── main.dart                    (Flutter source)
│   └── README.md
└── partD/
    └── CMPE258_Assignment1_PartD_MNIST.ipynb
```

---

## Part A: Multimodal AI with Google Gemini 🎨

### Description
A comprehensive Google Colab notebook demonstrating multimodal AI capabilities using Google's Gemini models (Gemini 2.5 Flash / 3 Flash / 2.0 Flash).

### Features Demonstrated
- **Text Conversations with Reasoning** – Step-by-step reasoning, creative story writing, and technical explanations using Gemini
- **Image Analysis (Upload)** – Upload your own image and analyze it with Gemini
- **Image Analysis (Generated)** – Create a sample image programmatically and analyze it
- **Image from URL** – Download and analyze images directly from URLs
- **Multimodal Creative Workflow** – Generate an artistic scene and get AI-powered descriptions
- **Visual Question Answering** – Ask natural language questions about image content using Gemini

### How to Run
1. Open the notebook in [Google Colab](https://colab.research.google.com/drive/1aZ-1-KYaDJkSQ9-HXDByyBLvJSXRRVDJ?usp=sharing)
2. Select **GPU runtime** (Runtime → Change runtime type → T4 GPU)
3. Configure your Gemini API key when prompted


## Part B: SpendWise AI - Smart Expense Tracker (Web App) 💰

### Description
A full-stack web application built as an AI-powered expense tracker with smart insights, interactive dashboard, and an AI chat assistant.

### UI/UX Design: Dark Cyberpunk Financial Dashboard
- **Theme:** Dark mode with neon accents (purple/teal)
- **Font:** DM Sans + Instrument Serif
- **Layout:** Grid-based dashboard with cards
- **Key Differentiator:** Professional financial dashboard feel with glowing elements

### Features
- ✅ Interactive expense/income tracking
- ✅ Real-time donut chart for category breakdown
- ✅ AI-powered smart insights (spending patterns, savings tips)
- ✅ AI Chat assistant for financial queries
- ✅ Add/manage transactions with modal
- ✅ CSV export functionality
- ✅ Responsive design (mobile + desktop)

### Tech Stack
- HTML5, CSS3 (Custom Properties, Grid, Flexbox)
- Vanilla JavaScript (no frameworks)
- AI Chat simulation (can be connected to Gemini API)

### Screenshots
*Dark dashboard with expense tracking, donut chart, and AI insights*

### How to Run
Open `spendwise-web-app.html` in any modern browser.

---

## Part C: MindFlow - AI Mood & Wellness Journal (Mobile App) 🧘

### Description
A cross-platform mobile application built with Flutter, featuring mood tracking, wellness journaling, and AI-powered insights using Google Gemini.

### UI/UX Design: Warm Organic Wellness Theme
- **Theme:** Light warm background (#FBF8F3) with colorful accents
- **Font:** Nunito + Playfair Display
- **Layout:** Card-based mobile-first with bottom navigation
- **Key Differentiator:** Soft, inviting wellness app feel (vs Part B's sharp financial dashboard)

### Design Differences from Part B (Web App)
| Aspect | Part B (SpendWise) | Part C (MindFlow) |
|--------|-------------------|-------------------|
| Theme | Dark cyberpunk | Light warm organic |
| Colors | Purple/Teal neon | Pastel/Soft gradients |
| Typography | DM Sans (modern) | Nunito (friendly rounded) |
| Layout | Grid dashboard | Card-based vertical scroll |
| Mood | Professional/corporate | Personal/wellness |
| Navigation | Top header + sidebar chat | Bottom tab bar + FAB |

### Features
- ✅ Daily mood check-in (5-point emoji scale)
- ✅ Journal entries with tags
- ✅ Wellness tracking (sleep hours, water intake, exercise)
- ✅ Weekly mood chart visualization
- ✅ AI-powered weekly summaries and insights
- ✅ Mood streak tracking
- ✅ Per-class mood analytics
- ✅ 4 pages: Home, Journal, Insights, Profile

### Tech Stack
- **Framework:** Flutter (Dart)
- **AI:** Google Gemini 2.0 Flash API
- **Charts:** fl_chart
- **Storage:** shared_preferences
- **Prototype:** HTML/CSS/JS (pixel-perfect Flutter-like design)

### How to Run
**Interactive Prototype:** Open `mindflow-mobile-app.html` in a mobile browser or use Chrome DevTools mobile view (430px width).

**Flutter App:**
```bash
cd partC/flutter_app
flutter pub get
flutter run
```

---

## Part D: MNIST Neural Network Classifier 🧠

### Description
A comprehensive Keras implementation of MNIST digit classification with three model architectures and extensive evaluation metrics, as demonstrated in class.
Colab: https://colab.research.google.com/drive/1am1Ovm2xR1P2L6BuwnFLWHY_gNrWnC8d?usp=sharing
### Models
| Model | Architecture | Key Features |
|-------|-------------|-------------|
| Dense Network | 784→256→128→10 | Baseline, dropout |
| Standard CNN | 2×Conv blocks + Dense | BatchNorm, MaxPool, Dropout |
| Advanced CNN | 3×Conv blocks + GAP | Data augmentation, L2 regularization, GlobalAveragePooling |

### Metrics & Visualizations
- ✅ Training/Validation accuracy & loss curves
- ✅ Confusion matrix (raw + normalized)
- ✅ Per-class precision, recall, F1-score
- ✅ Classification report
- ✅ ROC curves with AUC (per class)
- ✅ Precision-Recall curves with AP
- ✅ Model comparison table
- ✅ Misclassified samples analysis
- ✅ Prediction confidence distribution
- ✅ Grad-CAM visualization (what the CNN sees)
- ✅ Data augmentation examples

### Expected Results
| Model | Accuracy | Parameters |
|-------|----------|-----------|
| Dense Network | ~97-98% | ~235K |
| Standard CNN | ~99.2%+ | ~400K+ |
| Advanced CNN | ~99.4%+ | ~200K+ |

### How to Run
1. Open `CMPE258_Assignment1_PartD_MNIST.ipynb` in Google Colab
2. Select GPU runtime (Runtime → Change runtime type → GPU)
3. Run all cells

---

## 🛠️ Technologies Used

- **AI/ML:** Stable Diffusion, BLIP, CLIP, Gemma 2B, ViT, TensorFlow/Keras
- **Web:** HTML5, CSS3, JavaScript
- **Mobile:** Flutter/Dart
- **Data Science:** NumPy, Matplotlib, Seaborn, Scikit-learn, HuggingFace Transformers
- **Tools:** Google Colab (free GPU), Git/GitHub

---

## 📝 Notes

- All artifacts are checked into this GitHub repository
- Each part has a video walkthrough demonstrating the functionality
- Part B (Web) and Part C (Mobile) intentionally have **different UI/UX designs** to showcase variety
- Part A runs on Colab's free T4 GPU
