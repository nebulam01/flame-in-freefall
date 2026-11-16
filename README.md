# 🔥 Flame in Freefall: SI-Powered Fire Safety Insights from Microgravity Combustion Data

An interactive simulation and predictive analytics dashboard developed for the **2026 NASA Space Apps Challenge**. This platform evaluates combustion risks, droplet burning dynamics, and chemical extinction limits in microgravity environments, providing actionable engineering safety recommendations based on real NASA experimental data.

---

## 🚀 Key Features

* **NASA PSI Data Integration:** Built upon **75 experimental Excel datasets** (419,000+ data rows) sourced from NASA’s Physical Sciences Informatics (PSI) database.
* **Multi-Fuel Chemical Kinetics Engine:** Supports key reference fuels including **n-Dodecane ($C_{12}H_{26}$)**, **n-Heptane ($C_7H_{16}$)**, **n-Decane ($C_{10}H_{22}$)**, **Methanol ($CH_3OH$)**, and **Ethanol ($C_2H_5OH$)**.
* **Real-Time Parameter Simulation:** Evaluates combustion behavior across Pressure ($atm$), Oxygen Concentration ($X_{O_2}$), $CO_2$ Ratio, Nitrogen ($N_2$), Temperature ($K$), and Initial Droplet Diameter ($D_0$).
* **Automated Risk Assessment & Recommendations:** Classifies conditions into **Safe Zone (Self-Extinguishing Tendency)** or **High Risk (Elevated Flammability)** with scientific justifications, engineering safety recommendations, and nearest experimental record matching.
* **Interactive Trend Mapping:** Visualizes user inputs directly against NASA baseline curves (**Pressure Sweep** & **Oxygen Sweep**).

---

## 🛠️ Tech Stack

* **Environment:** Google Colab
* **Backend & Data Processing:** Python, Flask, Pandas, NumPy, Scikit-learn (Random Forest), OpenPyXL
* **Frontend & Visualization:** HTML5, CSS3, JavaScript, Chart.js

---

## ⚙️ How to Run in Google Colab

> **📌 Important Note:** To run this project properly, **you must download ALL project files (both the code files from this GitHub repository and all 75 Excel datasets from Google Drive) and upload them together into Google Colab.**

1. **Download All Required Files:**
   * **From GitHub:** Click the green **`<> Code`** button at the top of this page and select **Download ZIP** (or download **`NASA2026.ipynb`** and the **6 core project files** individually).
   * **From Google Drive:** Due to GitHub's 25 MB web file size limit, all **75 NASA PSI Excel datasets** (`.xlsx`) are stored in our Google Drive folder. Download all Excel files here: **[Download All 75 NASA PSI Excel Datasets (Google Drive)](BURAYA_DRIVE_LINKINI_YAPISTIR)**
2. **Upload Everything to Google Colab:**
   * Open **`NASA2026.ipynb`** in [Google Colab](https://colab.research.google.com/).
   * Click the **Files (📁)** icon on the left sidebar and upload **all downloaded files** (the **6 project files** + all **75 Excel `.xlsx` files**) directly into your Colab session storage.
3. **Install Dependencies & Run the Code:**
   * Run the dependency installation command in the first Colab cell:
     ```python
     !pip install flask flask-cors pandas numpy scikit-learn openpyxl
     ```
   * Run all remaining cells in **`NASA2026.ipynb`** to start the Flask server and open the interactive fire safety dashboard.

---

## 📄 Data Attribution & License

* **Dataset Source:** All 75 experimental microgravity combustion datasets used in this project are publicly available open-access data retrieved from the official **NASA Physical Sciences Informatics (PSI)** database ([psi.nasa.gov](https://psi.nasa.gov/)).
* **Project Code:** The source code, machine learning pipeline, and simulation dashboard developed by our team are open-source and intended for educational and research purposes.
