📈 Advanced Stock Portfolio Tracker

A Streamlit-powered real-time portfolio management and analytics dashboard

🌟 Overview

The Stock Portfolio Tracker is an interactive, data-driven portfolio management application built with Python, Streamlit, Plotly, and yFinance.
It allows users to add, monitor, and analyze stock holdings in real time using an intuitive and visually appealing dashboard.

This project is designed to help investors, learners, and finance enthusiasts track performance, visualize gains, and maintain a complete transaction history.

🚀 Key Features
🔹 Real-Time Price Tracking

Fetches live stock prices using the yfinance API with fallback default prices.

🔹 Portfolio Management

Add stocks with quantity and custom purchase price

Remove/change holdings

Auto-calculated average buy price

Real-time gain/loss tracking

🔹 Advanced Analytics & Visualization

Portfolio value over time (simulated history)

Allocation donut chart

Gain/Loss comparison chart

Auto-updating performance metrics

🔹 Transaction History

Complete BUY/SELL log

Amount, price, quantity, timestamps

Color-coded data table

🔹 Export Options

Export your portfolio to:

CSV

JSON (with full summary + transactions)

🔹 Streamlit UI Enhancements

Clean, professional dashboard

Sidebar actions

Responsive metrics layout

Light custom CSS styling

🖥️ Tech Stack
Component	Technology
Frontend	Streamlit
Backend	Python
Data Fetching	yFinance
Charts	Plotly (Graph Objects + Express)
Data Processing	Pandas, NumPy
📊 App Structure

The dashboard contains four main sections:

1️⃣ Portfolio Overview

Total value

Cost basis

Gain/Loss

Performance line chart

Allocation pie chart

2️⃣ Performance

Detailed metrics per stock

Gain % comparison

Allocation bars

3️⃣ Holdings

Full holdings table

Formatted values

Best performer

Avg gain%

4️⃣ Transactions

All BUY/SELL logs

Summary metrics

Styled table

📁 Project Structure
.
├── main.py          # Main Streamlit app
├── README.md        # Documentation
└── portfolio_export_*.csv/json files (generated)

▶️ Getting Started
✔ Requirements
Python 3.10+
Streamlit
pandas
numpy
yfinance
plotly

✔ Installation
pip install -r requirements.txt

✔ Run the App
streamlit run main.py

🧩 How to Use
➕ Add Stocks

Use the sidebar:

Enter symbol (e.g., AAPL, TSLA)

Enter quantity

(Optional) enter purchase price

➖ Remove Stocks

Select existing stock

Enter quantity to remove

📤 Export Portfolio

Choose CSV or JSON, then download with one click.

⚙️ Notes

This is a demo educational project, not financial advice.

Some historical data uses simulated randomness for chart visualizations.

💡 Future Enhancements

Real daily portfolio history tracking

Integration with real brokerage APIs

Email alerts for price movements

Multi-portfolio support

🤝 Contributing

Pull requests and improvements are welcome!
