# project4-eda

COVID-19 Exploratory Data Analysis (EDA)

📌 Project Overview

This project performs Exploratory Data Analysis (EDA) on COVID-19 data obtained from an API. The dataset contains information on daily reported cases, tests, hospitalizations, and deaths across different U.S. states. The analysis focuses on data cleaning, handling missing values, and visualizing key trends.

[🔗 Trello Board](https://trello.com/b/5LNZiRo7/eda-machine-learning)


📊 Data Source

The data is fetched from the COVID Tracking Project API. The dataset includes:

Daily reported positive and negative COVID-19 cases

Total tests conducted

Hospitalizations and deaths by state

📂 Files & Directories

covid19_eda.ipynb: Jupyter Notebook containing the full analysis

README.md: Documentation (this file)

requirements.txt: Required dependencies

data/: (Optional) Folder to store any local CSV files if needed

⚙️ Installation & Setup

To run this project on your local machine:

# Clone the repository
git clone https://github.com/your-username/covid19-eda.git
cd covid19-eda

# Create a virtual environment (optional but recommended)
python -m venv env
source env/bin/activate  # On Windows use: env\Scripts\activate

# Install dependencies
pip install -r requirements.txt

# Run the notebook
jupyter notebook

🔍 Data Preprocessing

1️⃣ Fetching & Loading Data

The dataset is retrieved directly from the API using requests.

It is converted into a pandas DataFrame.

The date column is formatted correctly (YYYY-MM-DD).

2️⃣ Handling Missing Data

Missing values are replaced with 0.

Only relevant columns are retained (date, state, positive, negative, hospitalizedCurrently, death, totalTestResults).

3️⃣ Data Exploration

Statistical Summary: Basic statistics like mean, min, and max are examined.

Data Visualization:

Line plots for trends in cases, tests, and hospitalizations.

Scatter plots to analyze correlations (e.g., hospitalizations vs. deaths).

Heatmaps to explore correlations between numerical variables.

📈 Key Insights

Trends Over Time:

The number of positive cases follows a fluctuating trend based on testing volume.

The total tests conducted increase over time, affecting case detection rates.

Correlation Analysis:

Strong correlation (0.66) between hospitalizations and deaths.

Testing numbers impact case detection, but positivity rates vary by state.

State-wise Impact:

The top 10 states with the highest deaths are visualized using bar plots.

Some states experienced sharper spikes in cases compared to others.

📌 Next Steps

Implement hypothesis testing to validate observed trends.

Extend analysis to compare different time periods.

Deploy an interactive dashboard using Plotly or Dash.

🛠 Technologies Used

Python (Pandas, NumPy, Matplotlib, Seaborn)

Jupyter Notebook

Requests (for API calls)

📜 License

This project is licensed under the MIT License.

🤝 Contributions

Contributions are welcome! Feel free to fork this repository and submit pull requests.

✉️ For any questions, contact mreza.shidfar@gmail.com .

