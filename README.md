Bar Inventory Forecasting and Recommendation System
Overview
This project addresses the critical challenge of optimizing inventory management for a multi-location bar operation within a hotel chain. By leveraging historical consumption data and advanced time series forecasting, the system aims to significantly reduce both stockouts (leading to lost sales and customer dissatisfaction) and overstocking (tying up capital and increasing waste).

Problem Solved
Traditional, manual inventory management often results in:

Lost Revenue: Due to stockouts of popular items.
Customer Dissatisfaction: When preferred drinks are unavailable.
Increased Costs: From emergency orders, spoilage, and excessive holding costs.
Operational Inefficiency: Manual processes are time-consuming and prone to error.
This system provides a data-driven solution to these problems by proactively recommending optimal inventory levels.

Key Features
AI-Powered Demand Forecasting: Utilizes the Prophet time series model to accurately predict future daily consumption for various alcohol types across different bar locations.
Dynamic Par Level Recommendations: Generates precise inventory par levels for each item, incorporating forecasted demand, supplier lead times, and a calculated safety stock.
Performance Simulation: Includes a simulation framework to evaluate the effectiveness of the recommended par levels against historical data, highlighting potential stockout or overstock events.
Robust Data Handling: Processes raw, granular consumption data (including different timestamps within a day) and aggregates it for time-series analysis.
Seasonality & Trend Capture: Prophet's capabilities ensure the model effectively accounts for daily, weekly, and yearly consumption patterns.
Technologies Used
Python: Core programming language.
Pandas: For data manipulation, cleaning, and aggregation.
Prophet (from Meta): For time series forecasting.
Matplotlib: For data visualization.
How to Use (Local Setup - Example)
Clone the repository:
Bash

git clone https://github.com/YourUsername/your-repo-name.git
cd your-repo-name
Install dependencies:
Bash

pip install pandas prophet matplotlib openpyxl
(Note: openpyxl is needed if you're directly reading .xlsx files)
Place your dataset: Ensure your Consumption Dataset.xlsx (or converted .csv file) is in the project directory.
Run the script: Execute the main Python script containing the analysis and forecasting logic.
Bash

python your_script_name.py
