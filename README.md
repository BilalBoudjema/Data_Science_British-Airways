# ✈️ British Airways Analytics & Machine Learning Portfolio

This repository centralizes two key Data Analysis and Machine Learning projects developed for British Airways, aiming to optimize operations, resources, and the overall customer experience.

Each project resides in a dedicated subfolder and includes its own detailed `README.md`.

---

## 💡 Included Projects

| Project | Primary Objective | Key Technologies | Folder |
| :--- | :--- | :--- | :--- |
| **Lounge Eligibility Modeling** | Estimate demand for airport lounges (Concorde, First, Club) to optimize space and resource planning at Heathrow Terminal 3. | Python, Pandas, Statistical Modeling (Lookup Tables) | [**`lounge-eligibility-model`**](./lounge-eligibility-model) |
| **Customer Booking Prediction** | Predict customer booking completion behavior using a Machine Learning model to identify key influencing factors. | Python, `scikit-learn`, Random Forest, Plotly, `python-pptx` | [**`customer-booking-prediction`**](./customer-booking-prediction) |

---

## 1️⃣ Lounge Eligibility Modeling

A flexible and scalable model designed to estimate passenger eligibility for British Airways' various **Airport Lounges**. The approach segments flights by time of day, type, and region to apply pre-calculated eligibility percentages.

### 🔑 Key Highlights

* **Resource Optimization:** Assists in lounge capacity planning and investment decisions.
* **Transparent Methodology:** Uses a simple **Lookup Table** for easy application to future flight schedules.
* **Fine-Grained Segmentation:** Flights are grouped by **Time of Day**, **Haul Type (Short/Long-haul)**, and **Destination Region**.

➡️ **For more details:** Read the [Lounge Eligibility Modeling project README](./lounge-eligibility-model/README.md).

---

## 2️⃣ Customer Booking Prediction

Implementation of a **Random Forest classification model** to predict whether a customer will complete their booking (`booking_complete`). The project focuses on model interpretability to reveal the key factors that influence the booking decision.

### 🔑 Key Highlights

* **Predictive Model:** Utilizes a **Random Forest Classifier** for high performance and feature insight.
* **Key Features:** Analysis based on `purchase_lead` time, length of stay, sales channel, and optional preferences (seat, meals, baggage).
* **Professional Deliverables:** Generates a comprehensive performance report and a PowerPoint presentation (`.pptx`) detailing metrics and feature importances.

➡️ **For more details:** Read the [Customer Booking Prediction project README](./customer-booking-prediction/README.md).

---

## 🚀 Repository Structure

```text
Data_Science_British-Airways/
├── customer-booking-prediction/
│   ├── Getting Started.ipynb      # Main Machine Learning Notebook (Task 2)
│   ├── README.md                  # Detailed README for Booking Prediction
│   └── outputs/                   # Generated charts, presentation, etc.
├── lounge-eligibility-model/
│   ├── README.md                  # Detailed README for Lounge Eligibility Model
│   └── data/                      # Input data, lookup tables, etc.
└── README.md                      # Main Repository README (High-level overview)
