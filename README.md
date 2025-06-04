# Customer Segmentation using K-Means Clustering

## 📌 Project Overview
This project implements a customer segmentation system using the K-Means clustering algorithm. It groups customers into distinct segments based on demographic and behavioral attributes like age, income, and spending score. This helps businesses understand their customer base better, enabling targeted marketing strategies and improved customer engagement.

---

## Key Features
- 🔍 Automated customer segmentation using K-Means clustering  
- 📈 Optimal cluster determination using the Elbow Method  
- 🖥️ Interactive web interface for data input and visualization  
- 📊 Comprehensive visualizations of customer segments  
- 🔐 User authentication system for secure access  

---

## 🛠️ Technologies Used
- **Backend**: Python, Flask  
- **Machine Learning**: Scikit-learn, Pandas, NumPy  
- **Database**: MySQL  
- **Visualization**: Matplotlib, Seaborn  
- **Frontend**: HTML, CSS, JavaScript  

---

## ⚙️ Installation and Setup

### Prerequisites
- Python 3.7 or higher  
- MySQL Server  
- pip (Python package installer)  

### Steps to Run the Project

1. **Clone the repository**:
   ```bash
   git clone https://github.com/yourusername/customer-segmentation.git
   cd customer-segmentation

2. **Install dependencies**:
   ```bash
   pip install -r requirements.txt

3. **Set up the database:**:
- Ensure MySQL server is running  
- Create a```.env```file in the project root with the following variables:
```bash
DB_HOST=localhost
DB_USER=your_mysql_username
DB_PASSWORD=your_mysql_password
DB_NAME=customer_segmentation
DB_PORT=3306
SECRET_KEY=your_secret_key_here
```
4. **Train the K-Means model:**:
   ```bash
   python clustering.py
  This will:
- Load the customer data 
- Preprocess the features
- Determine optimal clusters using the Elbow Method
- Train and save the K-Means model

5. **Run the application**:
   ```bash
   python app.py
   ```
6. **Access the application**:
Open a web browser and navigate to http://localhost:5000

---
## 🧑‍💼 Usage Instructions

### 🔐 Registration
- Navigate to the **Registration** page.
- Create an account by entering a **Username**, **Email**, and **Password**.
- Submit the form to register and log in.

---

### 🔑 Login
- Go to the **Login** page.
- Enter your registered credentials (**Email** and **Password**).
- Click **Login** to access the dashboard.

---

### 👤 Customer Segmentation
- On the **Dashboard**, input the following customer details:
  - **Age**
  - **Annual Income** (in thousands)
  - **Spending Score** (1–100)
- Click the **“Analyze Customer”** button.
- The system will use the trained **K-Means model** to classify the customer into a specific cluster.

---

### 📊 View Visualizations

#### 1️⃣ Income vs. Spending Score by Cluster
This scatter plot shows how customers are distributed based on income and spending behavior.

![Income vs. Spending Score](images/income_vs_spending.png)

---

#### 2️⃣ Age vs. Spending Score by Cluster
This visualization highlights spending patterns across different age groups.

![Age vs. Spending Score](images/age_vs_spending.png)

---

#### 3️⃣ Age vs. Annual Income by Cluster
This plot reveals income distribution across various age segments.

![Age vs. Income](images/age_vs_income.png)

---

#### 4️⃣ Cluster Distribution Overview
This bar chart shows the number of customers in each cluster.

![Cluster Distribution](images/cluster_distribution.png)
