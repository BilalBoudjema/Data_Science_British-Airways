# ✈️ British Airways Analytics & Machine Learning 

This repository centralizes two key Data Analysis and Machine Learning projects developed for British Airways, aiming to optimize operations, resources, and the overall customer experience.

Each project resides in a dedicated subfolder and includes its own detailed `README.md`.

---

## 💡 Included Projects

| Project | Primary Objective | Key Technologies | Folder |
| :--- | :--- | :--- | :--- |
| **Lounge Eligibility Modeling** | Estimate demand for airport lounges (Concorde, First, Club) to optimize space and resource planning at Heathrow Terminal 3. | Python, Pandas, Statistical Modeling (Lookup Tables) | [**`task-1-lounge-eligibility`**](./task-1-lounge-eligibility) |
| **Customer Booking Prediction** | Predict customer booking completion behavior using a Machine Learning model to identify key influencing factors. | Python, `scikit-learn`, Random Forest, Plotly, `python-pptx` | [**`task-2-booking-prediction`**](./task-2-booking-prediction) |

---

## 1️⃣ Lounge Eligibility Modeling (Task 1)

A flexible and scalable model designed to estimate passenger eligibility for British Airways' various **Airport Lounges**. The approach segments flights by time of day, type, and region to apply pre-calculated eligibility percentages.

### 🔑 Key Highlights

* **Resource Optimization:** Assists in lounge capacity planning and investment decisions.
* **Transparent Methodology:** Uses a simple **Lookup Table** for easy application to future flight schedules.
* **Fine-Grained Segmentation:** Flights are grouped by **Time of Day**, **Haul Type (Short/Long-haul)**, and **Destination Region**.

➡️ **For more details:** Read the [Lounge Eligibility Modeling project README](./task-1-lounge-eligibility/README.md).

---

## 2️⃣ Customer Booking Prediction (Task 2)

Implementation of a **Random Forest classification model** to predict whether a customer will complete their booking (`booking_complete`). The project focuses on model interpretability to reveal the key factors that influence the booking decision.

### 🔑 Key Highlights

* **Predictive Model:** Utilizes a **Random Forest Classifier** for high performance and feature insight.
* **Key Features:** Analysis based on `purchase_lead` time, length of stay, sales channel, and optional preferences (seat, meals, baggage).
* **Professional Deliverables:** Generates a comprehensive performance report and a PowerPoint presentation (`.pptx`) detailing metrics and feature importances.

➡️ **For more details:** Read the [Customer Booking Prediction project README](./task-2-booking-prediction/README.md).

---

## 🚀 Repository Structure
'''
Data_Science_British-Airways/
├── Task1/
│   └── (Files related to Lounge Eligibility Modeling)
├── Task2/
│   └── (Files related to Customer Booking Prediction)
└── README.md
'''
