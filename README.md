# Video Game Sale & Publisher Performance Analysis

An end-to-end data analysis and machine learning pipeline in Python exploring video game sales across different publishers, platforms, genres, and regional markets.

---

## 📌 Project Overview
This project generates a synthetic dataset mimicking the structure of the Kaggle `vgsales` dataset (500 records) to analyze publisher performance, regional market trends, and platform distributions. It also includes predictive modeling experiments to evaluate how well categorical metadata can predict global video game sales.

---

## 📊 Key Highlights & Insights

* **Top Publishers:** Analyzed global revenue generated across major industry publishers such as Sega, Capcom, Take-Two Interactive, Nintendo, Ubisoft, and Sony Computer Entertainment.
* **Regional Dynamics:** Compared total sales volume and distribution across North America (`NA_Sales`), Europe (`EU_Sales`), Japan (`JP_Sales`), and Other regions (`Other_Sales`).
* **Cross-Platform Distribution:** Mapped out publisher strategies, identifying platform performance variations across consoles (e.g., PlayStation, Xbox, Wii, DS).
* **Predictive Modeling Takeaways:**
  * Evaluated baseline regression models (**Random Forest Regressor** and **Ridge Regression**) using One-Hot Encoded features (`Platform`, `Genre`, `Publisher`).
  * Findings indicate that categorical metadata alone on randomly generated synthetic data produces low predictive power ($R^2 < 0$), highlighting the necessity of additional real-world variables like Critic/User scores, marketing budgets, release timing, and historical franchise performance.

---

## 🛠️ Dataset Features

| Column Name | Type | Description |
| :--- | :--- | :--- |
| `Rank` | Integer | Overall sales ranking |
| `Name` | String | Title of the game |
| `Platform` | String | Release console/device (e.g., Wii, PS4, XB, PC) |
| `Year` | Integer | Release year |
| `Genre` | String | Game category (e.g., Action, Sports, Platform) |
| `Publisher` | String | Game publisher |
| `NA_Sales` | Float | Sales in North America (in millions) |
| `EU_Sales` | Float | Sales in Europe (in millions) |
| `JP_Sales` | Float | Sales in Japan (in millions) |
| `Other_Sales` | Float | Sales in rest of the world (in millions) |
| `Global_Sales` | Float | Total world sales (in millions) |

---

## 💻 Tech Stack & Libraries

* **Python 3**
* **Data Processing & Manipulation:** `pandas`, `numpy`
* **Data Visualization:** `matplotlib`, `seaborn`
* **Machine Learning:** `scikit-learn` (`RandomForestRegressor`, `Ridge`, `train_test_split`, `metrics`)

---

## 🚀 Getting Started

### Prerequisites
Make sure you have Python installed along with the required libraries:

```bash
pip install pandas numpy matplotlib seaborn scikit-learn
