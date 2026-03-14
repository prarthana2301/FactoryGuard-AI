# FactoryGuard AI ⚙️

An AI-powered smart factory monitoring platform that integrates **Predictive Maintenance**, **Visual Quality Inspection**, and **Supply Chain Risk Management** into one unified web application.

Built as a Final Year Project using Python and Streamlit.

---

## Modules

### ⚙️ Module 1 — RUL Prediction (Predictive Maintenance)
- Predicts the **Remaining Useful Life** of industrial machines
- Uses **XGBoost Regressor** with 3 sensor readings, operational hours and maintenance count
- Classifies machines as Healthy, Warning or Critical
- R² Score: **0.9993**

### 🔍 Module 2 — Visual Inspection
- Detects **steel surface defects** from uploaded images
- Uses a **CNN (Convolutional Neural Network)** trained on the NEU Steel Surface Dataset
- Detects 6 defect types: Crazing, Inclusion, Patches, Pitted Surface, Rolled-in Scale, Scratches

### 📦 Module 3 — Supply Chain Risk Management
- Classifies supply orders as **High or Low risk**
- AI suggestions dynamically change based on real-time machine health from Module 1
- Saves full order history to database

---

## Tech Stack

| Layer | Technology |
|-------|-----------|
| Frontend | Streamlit |
| ML - RUL | XGBoost + Scikit-learn |
| ML - Vision | TensorFlow / Keras CNN |
| ML - Supply Chain | Scikit-learn |
| Charts | Plotly Express |
| Database | SQLite |
| Image Processing | Pillow |

---

## Project Structure
```
FactoryGuard-AI/
├── factory_ai/          # Main Streamlit application
│   ├── app.py           # Main app file
│   ├── requirements.txt # Dependencies
│   └── *.ipynb          # Model training notebooks
├── visual inspection/   # CNN model training notebooks
├── supply chain/        # Supply chain model notebooks
└── visual control/      # Visual control experiments
```

---

## How to Run

**1. Clone the repository**
```bash
git clone https://github.com/prarthana2301/FactoryGuard-AI.git
cd FactoryGuard-AI/factory_ai
```

**2. Install dependencies**
```bash
pip install -r requirements.txt
```

**3. Run the app**
```bash
streamlit run app.py
```

---

## Dataset

- **RUL Dataset** — Synthetic machinery sensor data (1000 samples)
- **Visual Inspection** — [NEU Steel Surface Defect Dataset](http://faculty.neu.edu.cn/yunhyan/NEU_surface_defect_database.html) (1800 images, 6 classes)
- **Supply Chain** — Custom order risk dataset

---

## Key Features

- Multi-user login with secure password hashing
- Real-time dashboard with KPI cards and charts
- Cross-module intelligence — machine health affects supply chain suggestions
- Full prediction history saved to SQLite database
- Analytics with trend detection and downloadable reports

---

## Model Files

Model files (`.pkl`, `.keras`) are not included due to size.
Run the training notebooks to generate them:
- `RUL_Model_Training.ipynb` — trains XGBoost RUL model
- `train_neu_defect_classifier.ipynb` — trains CNN visual inspection model
- `supply_chain_model.ipynb` — trains supply chain classifier

---
## Screenshots

!(D:\AI smart manufacturing\factory_ai\images\a5)




## Author

**Prarthana** | Final Year — Computer Science & Engineering | 2025
