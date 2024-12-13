# ballondorcalculator

### README for Ballon d'Or Analysis Project

# **Ballon d'Or Nominee Analysis: A Data-Driven Exploration**

## **Project Overview**
This project aims to analyze the performance and ranking of players nominated for the Ballon d'Or, one of the most prestigious awards in football. Using a dataset of player statistics, achievements, and advanced metrics, we created a dynamic, data-driven ranking system to explore how well the rankings align with players' on-field performance.

The project involves data cleansing, database storage, advanced analysis, and insightful visualizations, providing a comprehensive workflow from raw data to impactful insights.

---

## **Features**
- **Dynamic Ranking System**: Calculates player rankings based on a weighted scoring system tailored for different positions (forwards, midfielders, defenders).
- **Expected vs. Actual Performance**: Evaluates how players exceeded or underperformed based on expected goals (xG).
- **Visualization**: Interactive Tableau dashboards to visualize player rankings, performance trends, and metric correlations.
- **Database Integration**: Cleaned data stored in both SQL and MongoDB for scalability and structured querying.

---

## **Key Steps in the Project**
### 1. **Data Cleansing**
- Preprocessed a raw dataset containing statistics for Ballon d'Or nominees.
- Handled missing values and irrelevant data.
- Added key columns like `Rank`, `Total Points`, and `Gls_vs_xG` (Actual Goals vs. Expected Goals).

### 2. **Scoring and Ranking**
- Designed position-specific weighting systems:
  - **Forwards**: Emphasized offensive contributions like goals, assists, and expected metrics.
  - **Midfielders**: Balanced offensive and playmaking metrics with defensive contributions.
  - **Defenders**: Highlighted defensive metrics, recoveries, and aerial duels.
- Calculated total points and ranks dynamically using weighted scores for each player.

### 3. **Database Storage**
- Stored the cleansed and ranked dataset in:
  - **MongoDB**: For flexible, document-based storage.
- Provided schemas and data structures in a NoSQL database.

### 4. **Visualization in Tableau**
- Created interactive dashboards featuring:
  - Scatter plots of player rankings by total points.
  - Bar charts showing metric contributions to total scores.
  - Radar charts comparing players across multiple metrics.
  - Heatmaps illustrating correlations between performance metrics.

---

## **How to Use**
### Prerequisites:
- Install Python 3.x and required libraries (`pandas`, `numpy`, `sqlalchemy`, `pymongo`, `tableau`).
- Access to Tableau Desktop or Tableau Public for visualizations.

### Steps:
1. **Clone the Repository**:
   ```bash
   git clone https://github.com/amechi-aduba/ballondorcalculator.git
   ```

2. **Run the Data Processing Script**:
   - Open the `data_processing.py` script and execute it to:
     - Clean the data.
     - Calculate player scores and ranks.
     - Export the cleaned dataset (`ranked_table.csv`).

3. **Load the Data into a Database**:
   - Use `store_to_mysql.py` or `store_to_mongodb.py` scripts to upload the data to your chosen database.

4. **Visualize the Data**:
   - Import `ranked_table.csv` into Tableau.
   - Use the Tableau workbook (`visualizations.twbx`) to explore the dashboards.

---

## **Project Deliverables**
- **Python Code**: Includes data preprocessing, scoring, and database storage scripts.
- **Cleaned Dataset**: `ranked_table.csv` with calculated ranks and scores.
- **Tableau Visualizations**: Interactive dashboards showcasing player performance insights.
- **Database Integration**: MySQL and MongoDB schemas and stored data.

---

## **Contributions**
This project was developed as part of an end-to-end data analytics workflow. Contributions are welcome! Feel free to submit issues, feature requests, or pull requests.

---

## **License**
This project is licensed under the MIT License. See the `LICENSE` file for details.

---

## **Acknowledgments**
- Dataset inspired by Ballon d'Or 2024 statistics and initial results.
- Visualization tools provided by Tableau.
- Thanks to the football analytics community for inspiration.

---

Would you like me to customize the README further or generate specific sections, such as installation instructions?
