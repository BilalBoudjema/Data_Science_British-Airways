# Lounge Eligibility Modeling – British Airways

## 📌 Project Overview

This project estimates **passenger eligibility for airport lounges** (Concorde Room, First Lounge, and Club Lounge) at **Heathrow Terminal 3**. Lounge access is a key part of the premium travel experience, and forecasting lounge demand helps British Airways (BA) optimize space and resources while maintaining high service standards.

The model is **flexible and scalable**, allowing application to **future or changing flight schedules**.

---

## 🧭 Data

**Dataset:** British Airways Summer Schedule

- Total flights: 10,000  
- Key columns:
  - Flight date and time  
  - Departure and arrival airports  
  - Arrival region (Europe, North America, Asia, Middle East, Africa)  
  - Haul type (Short-haul / Long-haul)  
  - Aircraft type  
  - Seat distribution per class (First, Business, Economy)  

---

## 🧩 Methodology

### 1. Flight Grouping
Flights are grouped by:
- **Time of day:** Morning, Midday, Evening  
- **Route type:** Short-haul vs Long-haul  
- **Destination region:** Europe, North America, Asia, Middle East, Africa  

### 2. Lookup Table
Estimated **passenger eligibility percentages** per lounge tier:

| Grouping | Example Destinations | Tier 1 % | Tier 2 % | Tier 3 % |
|----------|--------------------|-----------|-----------|-----------|
| Short-haul – Morning – Europe | Paris, Frankfurt, Amsterdam | 0.5 | 1.5 | 8.0 |
| Short-haul – Midday – Europe | Madrid, Rome, Brussels | 0.3 | 1.0 | 6.0 |
| Short-haul – Evening – Europe | London, Berlin, Zurich | 0.4 | 1.2 | 7.0 |
| Short-haul – Premium Routes | London City, Frankfurt, Zurich | 0.8 | 3.0 | 12.0 |
| Long-haul – Morning – North America | New York, Toronto, Chicago | 1.0 | 5.0 | 20.0 |
| Long-haul – Midday – Middle East / Africa | Dubai, Johannesburg | 1.5 | 6.0 | 18.0 |
| Long-haul – Evening – Asia | Hong Kong, Singapore, Tokyo | 2.0 | 8.0 | 25.0 |

### 3. Assumptions
- **Tier 1 (Concorde Room):** Very limited, mainly top-tier loyalty members and first-class passengers.  
- **Tier 2 (First Lounge):** Small additional premium group; higher on long-haul flights.  
- **Tier 3 (Club Lounge):** Largest group, includes business class and silver/gold loyalty members.  

### 4. Application Steps
1. Assign flights to the appropriate category.  
2. Multiply passenger counts by lookup table percentages per tier.  
3. Aggregate results by day, region, or time window.  
4. Optional scenarios: conservative (-10%), baseline, optimistic (+10%).  

---

## 📊 Insights

- Afternoon long-haul flights (North America & Asia) have the **highest Tier 1 & 2 demand**.  
- Morning Europe short-haul flights have more business passengers (Tier 3 dominant).  
- Tier 3 demand is the **most stable and predictable**.  
- The lookup table is reusable for **any future flight schedule**.

---

## ⚡ Future Use

- Works with **changing schedules** or **new routes**.  
- Supports **lounge capacity planning** and **investment decisions**.  
- Percentages can be refined with **historical passenger data**.  

---

## 🛠️ Deliverables

1. **Lookup Table (CSV/Excel)** – category-wise Tier 1/2/3 percentages  
2. **Aggregated lounge eligibility summary** – by region and time of day  
3. Optional: **Heatmaps or bar charts** visualizing lounge demand  

---

## 🔧 Instructions for Use

1. Load the flight schedule dataset.  
2. Map each flight to its category (time of day, haul type, region).  
3. Apply the lookup table percentages to calculate eligible passengers per tier.  
4. Aggregate results for reporting or dashboard visualization.  

---

## 📌 Notes

- Tier 1 numbers are **hypothetical** for potential Concorde Room planning.  
- Lookup table is designed to be **flexible, conservative, and easy to justify** in internal reviews.  
- Adjust percentages based on **actual historical passenger data** when available.

---

