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

## ⚙️ How to Run the Project

> **📌 Important Note:** Due to GitHub's 25 MB web file size limit, the **main notebook (`NASA2026.ipynb` - zipped)** and all **75 NASA PSI Excel datasets** are hosted on Google Drive. To run this project, **download the files from both GitHub and Google Drive and open them together in Google Colab.**

1. **Download All Required Files:**
   * **From GitHub (6 Core Project Files):** Click the green **`<> Code`** button at the top of this page and select **Download ZIP**, then extract the 6 files.
   * **From Google Drive (Main Notebook + 75 Excel Datasets):** Download the zipped notebook (`NASA2026.ipynb`) and all **75 NASA PSI Excel datasets** (`.xlsx`) from our shared folder: **[Download Code & 75 Excel Datasets (Google Drive)](https://drive.google.com/drive/u/0/folders/1xipvwIipuFZkld-M6xa5a0lfJuJu1X1I)**
2. **Open in Google Colab:**
   * Extract the downloaded ZIP file from Google Drive to get **`NASA2026.ipynb`**.
   * Go to Google Colab (`colab.research.google.com`), click **File > Upload notebook**, and select **`NASA2026.ipynb`** from your computer.
   * Click the **Files (📁)** icon on the left sidebar and upload **all 6 project files from GitHub** along with **all 75 Excel (`.xlsx`) datasets** into your Colab session storage.
3. **Install Dependencies & Run:**
   * Run the dependency installation command in the first cell:
     ```python
     !pip install flask flask-cors pandas numpy scikit-learn openpyxl
     ```
   * Run all remaining cells in **`NASA2026.ipynb`** to start the Flask server and launch the interactive fire safety dashboard.

---

## 📄 Data Attribution & License

* **Dataset Source:** All 75 experimental microgravity combustion datasets used in this project are publicly available open-access data retrieved from the official **NASA Physical Sciences Informatics (PSI)** database ([psi.nasa.gov](https://psi.nasa.gov/)).
* **Project Code:** The source code, machine learning pipeline, and simulation dashboard developed by our team are open-source and intended for educational and research purposes.
