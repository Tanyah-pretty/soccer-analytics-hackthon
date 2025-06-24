# ⚽ Smart Sub Coach: AI-Powered Substitution Recommender for Football Matches

## 🚀 Overview

**Smart Sub Coach** is an intelligent substitution recommender system developed for the **Educait Soccer Analytics Hackathon 2.0**. This AI-driven solution analyzes real-time and historical player performance data to suggest **optimal substitutions** during a match.

The system goes beyond basic fatigue tracking by combining in-game performance dips, match context, and tactical awareness to **recommend when and who to sub**, helping coaches make smarter, data-backed decisions.

---

## 🎯 Problem Statement

In football, poorly timed or missed substitutions can cost teams valuable points. Coaches often rely on instinct, but:
- How can we **objectively measure player fatigue or underperformance**?
- When is the **best moment to make a substitution**?
- Who should be subbed **in or out** based on performance trends?

**Smart Sub Coach** solves this by using AI to analyze match stats and provide precise, explainable substitution suggestions.

---

## 💡 Solution Highlights

### ✅ Inputs:
- Player statistics: passes, tackles, distance covered, sprint rate
- Match context: yellow/red cards, current scoreline, game phase
- Time-series trend data from EPL matches (from Educait GitHub repo)

### 🔄 System Flow:
1. Monitor in-game player performance over time
2. Detect performance drop-offs or risk factors (e.g., yellow card, fatigue)
3. Recommend substitutions based on logic or model predictions
4. Provide clear justifications for each sub (e.g., “75th min: Player A’s accuracy dropped 20%”)

---

## 🛠 Tech Stack

| Component       | Tools / Libraries           |
|----------------|-----------------------------|
| Language        | Python                      |
| Data Handling   | Pandas, NumPy               |
| Modeling        | Scikit-learn, XGBoost       |
| Visualization   | Matplotlib, Seaborn, Plotly |
| Video Integration (optional) | OpenCV, moviepy     |
| Dashboard (optional) | Streamlit or Flask         |

---

## 📂 Project Structure

bash
📁 smart-sub-coach/
│
├── 📁 data/                   # EPL match & player data
├── 📁 notebooks/              # Exploratory analysis and modeling
├── 📁 src/                    # Core scripts (sub logic, evaluation)
├── 📁 visualizations/         # Charts and recommendation timelines
├── 📁 videos/ (optional)      # Clips linked to player fatigue/impact
├── requirements.txt
├── README.md
└── app.py                    # (Optional) dashboard or demo UI
`

---

## 📊 Sample Output

**Substitution Suggestion Timeline**:


Minute 68 → SUB: Replace Midfielder #8 with #14
Reason: Pass accuracy dropped from 88% → 62%, + yellow card + high opponent press


**Post-Match Report**:

* Sub made at 75’ had a +0.6 xImpact score (expected impact on match)
* Missed sub opportunity at 63’ (defender sprint rate collapsed)

---

## 🧪 How to Run

1. Clone the repo:

   bash
   git clone https://github.com/yourusername/smart-sub-coach.git
   cd smart-sub-coach
   

2. Install dependencies:

   bash
   pip install -r requirements.txt
   

3. Run core script:

   bash
   python src/substitution_recommender.py
   

4. (Optional) Launch interactive demo:

   bash
   streamlit run app.py
   

---

## 🎥 Demo Video

📺 Watch the short demo here:
[🔗 Google Drive Folder](https://drive.google.com/drive/folders/1ggxvNFesKVJ6bTad4LE1sjg3IWn3IvYL?usp=drive_link)

---

## 👨‍💻 Team

* **Shallin T Tairo** – ML & Performance Modeling, Feature Engineering, UI

---

## 📅 Submission Info

* **Challenge**: Educait Soccer Analytics Hackathon – Campus Creator Challenge 2.0
* **Submission Deadline**: June 24, 2025


