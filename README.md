# 🧠 BMI Analysis using MySQL and Python

A health-focused data analysis project to evaluate and classify individuals based on their Body Mass Index (BMI), using data stored in a MySQL database and processed with Python. The project calculates gender statistics, classifies BMI categories, and visualizes health distribution using histograms.

---

## 📌 Project Features

- Connects to a **MySQL** database to retrieve BMI records.
- Calculates:
  - Total individuals
  - Gender counts (Male/Female)
  - Gender-wise percentage distribution
- Classifies individuals into **BMI health categories**.
- Visualizes BMI distribution via a histogram using `matplotlib`.
- Saves chart as an image (`output.jpg`) and prints clean data tables.

---

## 🏥 Why BMI Analysis Matters (Especially in India)

In India, both **malnutrition and obesity** coexist:
- Rural areas often suffer from **underweight** due to poverty and lack of nutrition.
- Urban areas face growing rates of **obesity** due to sedentary lifestyle and fast food habits.
This project helps identify such disparities and can be integrated into **healthcare awareness tools** or screening programs.

---

## 🛠️ Technologies Used

- **Python 3.x**
- **MySQL** (Database)
- **Libraries**:
  - `MySQLdb` (mysqlclient)
  - `pandas`
  - `matplotlib`
  - `seaborn` (optional, for advanced visuals)

---

## 🧱 Database Schema

**Table Name**: `data`

| Column Name | Description          |
|-------------|----------------------|
| Gender      | Male or Female       |
| Height_m    | Height in meters     |
| Weight_kg   | Weight in kilograms  |
| BMI         | Body Mass Index      |
| Index       | BMI health category (0 to 5) |

**BMI Index Mapping**:
| Index | Status             |
|-------|--------------------|
| 0     | Extremely Weak     |
| 1     | Weak               |
| 2     | Normal             |
| 3     | Overweight         |
| 4     | Obesity            |
| 5     | Extreme Obesity    |

---

## 📈 Sample Output

- Total number of people
- Total males and females
- Percentage distribution by gender
- BMI status column added to dataset
- Histogram (saved as `output.jpg`)

---

## 📊 Visualization

<p align="center">
  <img src="output.jpg" alt="BMI Histogram" width="600">
</p>

---

## 🧪 How to Run the Project

### ✅ Prerequisites
- MySQL Server installed and running
- Python 3.x installed
- Dataset added to MySQL database named `bmi`, table named `data`
- Install required Python packages:
  ```bash
  pip install mysqlclient pandas matplotlib seaborn
