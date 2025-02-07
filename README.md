# 🚀 IBM Data Science Capstone Project - SpaceX  

![SpaceX Rocket Launch](https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBMDeveloperSkillsNetwork-DS0701EN-SkillsNetwork/api/Images/landing_1.gif)  

## 📌 Introduction  
SpaceX, a leader in the space industry, is revolutionizing space travel by making rocket launches more affordable. One of its key innovations is **reusing the first stage of the Falcon 9 rocket**, significantly reducing launch costs compared to competitors.  

In this capstone, we will predict if the **Falcon 9 first stage will land successfully**. SpaceX advertises Falcon 9 rocket launches on its website, with a cost of **62 million dollars**; other providers cost **upward of 165 million dollars** each. Much of the savings come from SpaceX’s ability to **reuse the first stage** of the rocket. Therefore, if we can determine **whether the first stage will land**, we can estimate the **cost of a launch**. This information can be useful if **an alternate company** wants to bid against SpaceX for a rocket launch.  

## 🎯 Objectives  
- Predict the success of a rocket's **first stage landing**.  
- Identify key factors influencing launch success.  
- Apply **exploratory data analysis (EDA)**, **visualization**, and **machine learning** techniques.  

---

# 📊 Executive Summary  
To achieve the objective, we followed these steps:  
✅ **Data Collection**: Obtained launch data via **SpaceX API** and **web scraping** (Wikipedia).  
✅ **Data Wrangling**: Cleaned and transformed data into a usable format.  
✅ **Exploratory Data Analysis (EDA)**: Visualized trends in launch success.  
✅ **Predictive Modeling**: Applied **Logistic Regression, Decision Tree, SVM, and KNN** models to predict landing success.  
✅ **Performance Evaluation**: Compared models based on accuracy, F1-score, and Jaccard index.  

---

# 📌 Results  

## 🔎 Exploratory Data Analysis  
- **Launch success rate increased over the years**, with more flights leading to better success rates, indicating **steady progress**.  
- **Orbits ES-L1, SSO, HEO, and GEO** had **high success rates**.  
- **KSC LC-39A** was the **launch site with the highest success rate**.  
- **FT booster version category** had the **highest success rate** among all booster versions.  

## 📈 Visualization & Analytics  
- **Most launch sites are near the equator and the coast** (for fuel efficiency and safety).  
- **Interactive Maps:** View launch sites and success rates on an interactive map  
  **➡ [Launch Site Locations (View Maps)](https://nbviewer.org/github/OmarHani4306/Applied-Data-Science-Capstone/blob/main/lab_jupyter_launch_site_location.ipynb)**  

## 🧠 Predictive Modeling  
- **Logistic Regression and Decision Tree** models were effective in predicting **landing success**.  
- **Dashboard App:** Visualize launch data insights interactively using Plotly Dash  
  **➡ [Dashboard Application (View App)](https://nbviewer.org/github/OmarHani4306/Applied-Data-Science-Capstone/blob/main/Build%20a%20Dashboard%20Application%20with%20Plotly%20Dash.ipynb)**  

---

# ⚙️ Methodology  

## 📡 Data Collection  
✅ **SpaceX API**  
- Extracted launch details using API requests.  
- Transformed JSON data into a Pandas DataFrame.  
- Filtered **only Falcon 9** launches.  

✅ **Web Scraping (Wikipedia)**  
- Extracted Falcon 9 launch data using **BeautifulSoup**.  
- Parsed HTML tables into structured data.  

## 🛠 Data Processing  
- Converted launch **outcomes to binary (1 = Success, 0 = Failure)**.  
- Filled missing **payload mass values** with the mean.  
- Exported clean data to CSV.  

## 🔍 EDA & Visualization  
- **SQL Queries**: Analyzed success rates by launch site and payload.  
- **Folium Maps**: Plotted **launch site locations** and their proximity to important landmarks.  
- **Plotly Dash**: Created interactive **dashboards** with:  
  - Pie charts (successful vs. failed launches).  
  - Scatter plots (Payload Mass vs. Success Rate).  

## 🤖 Machine Learning Models  
Applied **4 supervised learning models** to predict landing success:  
1️⃣ **Logistic Regression**  
2️⃣ **Decision Tree**  
3️⃣ **Support Vector Machine (SVM)**  
4️⃣ **K-Nearest Neighbors (KNN)**  

🔹 **Model evaluation metrics**: **Accuracy, F1-score, Jaccard index**.  
🔹 Used **GridSearchCV** for hyperparameter tuning.  

---

# ✅ Conclusion  

📌 **Success Rate Increased**: Over the years, more flights led to better success rates, showing **continuous progress**.  
📌 **High Success Orbits**: ES-L1, SSO, HEO, and GEO had **high success rates**.  
📌 **Best Launch Site**: **KSC LC-39A** had the **highest success rate**.  
📌 **Best Booster Version**: The **FT booster version** had the highest success rate.  
📌 **Predictive Models**: **Logistic Regression and Decision Tree** were effective in predicting **landing success**.  

---
 
