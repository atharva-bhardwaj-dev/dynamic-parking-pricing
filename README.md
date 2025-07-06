# Dynamic Parking Pricing 🚗💰

This project implements dynamic pricing strategies for smart parking using real-world parking data. The goal is to adaptively adjust parking rates based on demand, occupancy, and competition.

## 👨‍💻 Author
- Name: Atharva Bhardwaj
- Email: abhardwaj0624@gmail.com

## ⚙️ Tech Stack
- Python
- Google Colab
- Pandas, NumPy
- scikit-learn
- Pathway (streaming simulation)
- Haversine (distance-based pricing)

## 🧠 Models Implemented
1. **Baseline Linear Pricer**  
2. **Demand-Based Pricer**
3. **Competitive Pricer**

Each model was run on a real dataset with preprocessed time-based occupancy, queue length, and vehicle types.

## 🧱 Architecture Diagram

```mermaid
flowchart TD
    A[Raw CSV Data] --> B[Feature Engineering]
    B --> C[Baseline Model]
    B --> D[Demand Model]
    B --> E[Competitive Model]
    C --> F[Predicted Prices]
    D --> F
    E --> F
    F --> G[Saved CSV Output]
