# Hi, I'm Angela 👋

**Data and Analytics Professional | AI • Machine Learning • Business Intelligence**

I bring 15+ years of domain expertise in banking and financial services, combined with a self-built portfolio in Machine Learning, Generative AI, and Business Intelligence — developed through rigorous independent project work and formal study.

Currently at Accenture Technology Solutions (Kuala Lumpur), with hands-on exposure to AI/ML data operations. Holding a U.S.-accredited Master of Data Science (Birchwood University) with certifications from Stanford, AWS, Johns Hopkins, and Microsoft.

This GitHub documents my project work — every repo includes full code, documentation, and honest results.

- 🏦 15+ years in banking & financial services — strong domain advantage for fintech and financial analytics roles
- 🤖 Project focus: RAG systems, LLMs, Computer Vision, Predictive ML
- 📊 BI tools: Power BI (DAX), Tableau — from financial dashboards to model deployment
- 🎓 MDS — Birchwood University (U.S.-Accredited) | Stanford ML Specialization | AWS Cloud Practitioner | Johns Hopkins
- 📍 Kuala Lumpur, Malaysia | Open to SEA & U.S. opportunities

---

## 🛠️ Tech Stack

**Languages & Query:** Python, R, SQL, DAX, Power Query

**AI & Machine Learning:** TensorFlow, PyTorch, Scikit-learn, LangChain, LlamaIndex, OpenAI API, Hugging Face, Ollama

**BI & Visualization:** Power BI, Tableau

**Cloud & DevOps:** AWS, Docker, FastAPI, Flask, Streamlit

---

## 📂 Projects

### 🏦 Banking Loan Analytics — One Dataset, Five Business Questions

Most portfolios show one model solving one problem. This series does what a real banking analytics role actually demands: **the same 45,000-row loan dataset, interrogated from five different business angles** — each with its own target variable, its own leakage risks to audit, and its own algorithm family, because a real bank doesn't ask one question about its loan book, it asks several, and each one changes what "correct" data handling even means.

| Project | Type | Business Question | Tech | Result |
|---|---|---|---|---|
| [bank-loan-amount-prediction](https://github.com/angelaadida/bank-loan-amount-prediction) | Regression | How much should this customer be approved to borrow? | RandomForest, StandardScaler, RandomizedSearchCV, Tableau | R² 0.20, MAE $4,382 |
| [bank_loan-default-prediction](https://github.com/angelaadida/bank_loan-default-prediction) | Binary Classification | Will this customer default on the loan? | Logistic Regression, RandomForest, XGBoost | AUC-ROC 0.94, 90% default recall |
| [bank_loan-intent-classification](https://github.com/angelaadida/bank_loan-intent-classification) | Multi-class Classification | Why is this customer borrowing? | Logistic Regression, RandomForest | F1-macro 0.20 — honest negative result |
| [bank_interest-rate-prediction](https://github.com/angelaadida/bank_interest-rate-prediction) | Regression | What interest rate should be offered? | RandomForest, RandomizedSearchCV, Tableau | R² 0.09 — directional, not precise |
| [bank_customer-risk-segmentation](https://github.com/angelaadida/bank_customer-risk-segmentation) | Unsupervised Clustering | What natural customer groups exist, with no target at all? | KMeans, DBSCAN, PCA | 2 clean segments, silhouette 0.38 |

Same rows, same columns, five different meanings — and that's the point. `loan_amnt` is leakage when *predicting the loan amount itself*, but a legitimate input when *pricing the interest rate*. A 90% recall matters enormously when the question is default risk, and would be meaningless for a clustering problem that has no "correct" label to recall at all. Two of the five models above return weak R²/F1 scores — those are reported as-is, with the reasoning for *why* the data can't support a stronger answer, rather than tuned until the number looks better. Every notebook follows the same audited pipeline (leakage check → encode once → split → scale on train only → evaluate out-of-sample), because the discipline has to hold regardless of which of the five questions is being asked.

---

### 📊 Business Intelligence & Financial Analytics

| Project | Description | Tech |
|---|---|---|
| [financial-analytics-dashboard](https://github.com/angelaadida/financial-analytics-dashboard) | 15-page Financial Analytics Dashboard — P&L, Balance Sheet, Cash Flow, DuPont, Break-Even | Power BI, DAX |

---

### 🟢 Machine Learning — Supervised Learning

| Project | Type | Description | Tech | Result |
|---|---|---|---|---|
| [breast-cancer-gradient-xgboost](https://github.com/angelaadida/breast-cancer-gradient-xgboost) | Classification | Binary classification on Wisconsin dataset | GradientBoosting, XGBoost | 97% |
| [handwritten-digits-classification](https://github.com/angelaadida/handwritten-digits-classification) | Classification | Digit recognition — SVM vs RF vs DT | SVM, RandomForest | 97.5% |
| [earthquake-classification](https://github.com/angelaadida/earthquake-classification) | Classification | Tsunami prediction with hyperparameter tuning | RandomForest, GridSearchCV | 91% |
| [wine-adaboost-classification](https://github.com/angelaadida/wine-adaboost-classification) | Classification | Wine cultivar classification on 13 chemical features | AdaBoost | 92% |
| [housing-price-prediction](https://github.com/angelaadida/housing-price-prediction) | Regression | California housing regression | RandomForest | R²=0.80 |
| [earthquake-magnitude-regression](https://github.com/angelaadida/earthquake-magnitude-regression) | Regression | 42 models benchmarked with LazyPredict | RandomForest, GridSearchCV | R²=0.84 |
| [boston-housing-price-prediction](https://github.com/angelaadida/boston-housing-price-prediction) | Regression | Housing price prediction — 3 models compared | LinearRegression, RF, GradientBoosting | R²=0.907 |
| [career-level-classification](https://github.com/angelaadida/career-level-classification) | Classification | Job career level classification from text | NLP, RandomForest, SMOTEN | 73% |
| [diabetes-classification](https://github.com/angelaadida/diabetes-classification--) | Classification | Binary classification for diabetes prediction | RandomForest, GridSearchCV | 79% |
| [co2-direct-forecasting](https://github.com/angelaadida/co2-direct-forecasting) | Regression | CO₂ multi-step time series — Direct strategy | Direct Strategy, LinearRegression | R²=0.99/0.95/0.89 |
| [co2-recursive-forecasting](https://github.com/angelaadida/co2-recursive-forecasting) | Regression | CO₂ time series — Recursive strategy | Recursive Strategy, LinearRegression | R²=0.99 |
| [student-score-regression](https://github.com/angelaadida/student-score-regression) | Regression | Student math score prediction | LinearRegression, Pipeline | R²=0.88 |

---

### 🟣 Machine Learning — Unsupervised Learning

| Project | Type | Description | Tech | Result |
|---|---|---|---|---|
| [movie-recommendation-system](https://github.com/angelaadida/movie-recommendation-system) | Content-Based | Movie recommendation on MovieLens dataset | TF-IDF, Cosine Similarity | 9,742 movies |
| [mnist-pca-dimensionality-reduction](https://github.com/angelaadida/mnist-pca-dimensionality-reduction) | Dimensionality Reduction | PCA on 70K MNIST images | PCA, NumPy | 784→100 dims, 90%+ variance retained |
| [earthquake-kmeans-clustering](https://github.com/angelaadida/earthquake-kmeans-clustering) | Clustering | Earthquake pattern clustering | KMeans, PCA | Silhouette=0.27 |
| [earthquake-hierarchical-clustering](https://github.com/angelaadida/earthquake-hierarchical-clustering) | Clustering | Hierarchical clustering with dendrogram | Agglomerative, SciPy | Silhouette=0.23 |
| [earthquake-dbscan-clustering](https://github.com/angelaadida/earthquake-dbscan-clustering) | Clustering | Density-based clustering & noise detection | DBSCAN | Silhouette=0.29 |

---

### 🟠 Deep Learning & Computer Vision

| Project | Description | Tech |
|---|---|---|
| [football-detection-yolov5](https://github.com/angelaadida/football-detection-yolov5) | Player and ball detection from match videos | YOLOv5, COCO format, OpenCV |
| [object-detection-faster-rcnn-voc](https://github.com/angelaadida/object-detection-faster-rcnn-voc) | Object detection on PASCAL VOC 2012 — full training + inference pipeline | Faster RCNN, MobileNetV3, PyTorch |
| [semantic-segmentation-deeplabv3](https://github.com/angelaadida/semantic-segmentation-deeplabv3) | Pixel-level segmentation on PASCAL VOC 2012 — 21 classes | DeepLabV3, ResNet50, PyTorch |
| [football-segmentation-sam3](https://github.com/angelaadida/football-segmentation-sam3) | Pixel-level player segmentation in match videos via text prompt | SAM3, Ultralytics, OpenCV |
| [football-player-number-recognition](https://github.com/angelaadida/football-player-number-recognition) | Jersey number recognition (1–11) from match video | MobileNetV2, Transfer Learning |
| [Animal-Image-Classification](https://github.com/angelaadida/Animal-Image-Classification-) | Image classification on 10 animal categories — 3 models compared | AdvancedCNN, ResNet18, MobileNetV2 |
| [cifar10-image-classification](https://github.com/angelaadida/cifar10-image-classification) | Image classification from scratch on CIFAR-10 | MLP, SimpleCNN, AdvancedCNN, PyTorch |

---

### 🔵 Generative AI & LLMs

| Project | Description | Tech |
|---|---|---|
| [rag-pdf-question-answering](https://github.com/angelaadida/rag-pdf-question-answering) | RAG system for PDF Q&A — answers grounded strictly in provided documents | LangChain, FAISS, OpenAI GPT |
| [llm-local-ollama](https://github.com/angelaadida/llm-local-ollama) | Local LLM text generation + image understanding — offline, private | Ollama, LLaMA 3.1 8B, LLaMA 3.2 Vision 11B |
| [llm-serving-vllm](https://github.com/angelaadida/llm-serving-vllm) | High-throughput LLM serving with OpenAI-compatible API | vLLM, Qwen2.5-1.5B |
| [llm-inference-openai](https://github.com/angelaadida/llm-inference-openai) | LLM text generation via OpenAI Responses API | OpenAI GPT |
| [text-embedding](https://github.com/angelaadida/text-embedding) | Text embedding + cosine similarity — cloud and local | OpenAI, Ollama, FAISS |

---

### 🚀 Deployment & Web Apps

| Project | Description | Tech |
|---|---|---|
| [Image-Classification-with-ResNet50](https://github.com/angelaadida/Image-Classification-with-ResNet50) | Image classification web app — top-3 ImageNet predictions | ResNet50, Streamlit |
| [Image-Classification-with-ResNet101](https://github.com/angelaadida/Image-Classification-with-ResNet101) | Image classification web app | ResNet101, Streamlit |
| [Flask_CNN](https://github.com/angelaadida/Flask_CNN) | Fashion MNIST CNN model deployed as interactive web app | TensorFlow/Keras, Flask |

---

## 📫 Connect

[![LinkedIn](https://img.shields.io/badge/LinkedIn-blue?style=flat&logo=linkedin)](https://www.linkedin.com/in/angelaadida)
[![GitHub](https://img.shields.io/badge/GitHub-black?style=flat&logo=github)](https://github.com/angelaadida)
