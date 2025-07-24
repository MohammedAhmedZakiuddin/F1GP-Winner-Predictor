# 🏎️ F1 Predictions 2025 – Machine Learning Model

Welcome to **F1 Predictions 2025**!  
This project uses machine‑learning techniques, the FastF1 API, and historical Formula 1 race data to predict race outcomes for the 2025 season.

---

## 🚀 Project Overview
A Gradient Boosting model is trained on past performance, qualifying times, and structured F1 telemetry to forecast race results.

Key ingredients:

- **FastF1 API** – historical lap times, race results, telemetry  
- **2024 race results** – training data  
- **2025 qualifying sessions** – real‑time features  
- Feature‑engineering tricks to squeeze every millisecond of insight

---

## 📊 Data Sources
| Source | Purpose |
|--------|---------|
| **FastF1 API**            | Lap times, race results, telemetry |
| **2025 Qualifying data**  | Live features for predictions |
| **Historical results 2024** | Model training baseline |

---

## 🏁 How It Works
1. **Data Collection** – Pull fresh data from FastF1  
2. **Pre‑processing & Feature Engineering** –  
   - Convert lap times to numeric  
   - Normalise driver/team names  
   - Aggregate session information  
3. **Model Training** – Gradient Boosting Regressor on 2024 results  
4. **Prediction** – Forecast lap/race times and rank drivers  
5. **Evaluation** – Mean Absolute Error (MAE)

---

## 📦 Dependencies
- fastf1
- numpy
- pandas
- scikit-learn
- matplotlib

```bash
pip install fastf1 numpy pandas scikit-learn matplotlib
```

## File Structure
- For every race the end of the file will be numbered in correlation to the race on the calendar, ex. prediction1 - Australia, prediction2 - China, etc.

## 🔧 Usage

### Example: generate predictions for the Australian GP
```bash
python3 prediction1.py
```

```text
🏁 Predicted 2025 Australian GP Winner 🏁
Driver: Charles Leclerc | Predicted Race Time: 82.67 s
...
🔍 Model MAE: 3.22 seconds
```

## 📈 Model Performance
The Mean Absolute Error (MAE) is used to evaluate how well the model predicts race times. Lower MAE values indicate more accurate predictions.

## 📌 Future Improvements
- Introduce **weather conditions** as model features  
- Add **pit‑stop strategy** variables  
- Experiment with **deep‑learning** architectures for further gains.

---

## 📜 License
This project is licensed under the **MIT License**.

---

🏎️ **Start predicting F1 races like a data scientist!** 🚀

