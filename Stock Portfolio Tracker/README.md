📈 Advanced Stock Portfolio Tracker

A modern, intuitive, and analytics-driven stock portfolio management application built with Python and Streamlit. This tool helps users track real-time stock performance, analyze portfolio metrics, manage holdings, and visualize gains through beautifully designed charts and dashboards.

⭐ Features
📊 Real-Time Portfolio Tracking

Live stock prices via Yahoo Finance

Auto-calculated gain/loss

Total value, cost basis & performance metrics

➕ Portfolio Management

Add stocks with symbol, quantity, purchase price

Remove/sell holdings fully or partially

Automatic average price recalculation

Tracks purchase history & timestamps

📈 Visual Performance Analytics

Portfolio value chart (1W, 1M, 3M, 6M, 1Y, All)

Allocation donut chart

Gain/Loss comparison bar graph

Mini progress bars for stock allocation

🔄 Transaction History

Fully detailed BUY/SELL logs

Time-stamped entries

Color-coded actions

Summary: Buy/Sell ratio, total volume

📤 Data Export

Export portfolio to CSV

Export full portfolio + transactions to JSON

One-click download from sidebar

🎨 Streamlit UI/UX Enhancements

Clean responsive layout with custom CSS

Organized sidebar for quick actions

Tab-based navigation (Overview, Performance, Holdings, Transactions)

Smooth charts using Plotly

🛠️ Tech Stack
Component	Technology
Frontend	Streamlit
Backend	Python 3.x
Charts	Plotly (Graph Objects + Express)
Data Source	yFinance
Processing	Pandas, NumPy
State Storage	Streamlit Session State
📦 Installation
✔ Requirements

Python 3.8+

pip package manager

Internet connection (for live stock prices)

✔ Install Dependencies
pip install -r requirements.txt

✔ Run the App
streamlit run main.py

✔ Access the App

Visit:

http://localhost:8501

🚀 Usage Guide
➕ Add Stocks

Enter stock symbol (AAPL, TSLA, etc.)

Enter quantity

Optional: purchase price

Click Add to Portfolio

➖ Remove/Sell Stocks

Select a stock

Enter quantity

Click Remove from Portfolio

📊 View Performance

Explore charts under Portfolio Overview

Switch time periods (1W–1Y)

Analyze gain/loss across stocks

📋 View Holdings

Detailed table with:

Avg price

Current value

Cost basis

Gain %

Gain/Loss amount

🔄 View Transactions

Full BUY/SELL history

Color-coded action column

Summary metrics

📤 Export Data

Choose CSV or JSON

Download with one click

🗂️ Project Structure
stock-portfolio-tracker/
│
├── main.py               # Main Streamlit application
├── README.md             # Project documentation
└── requirements.txt      # Dependencies

🔒 Reliability & Data Handling

Fallback default prices if API fails

Prevents invalid quantity removal

Clean formatting for currency values

Session-based storage (no external database needed)

🎨 UI & Styling

Custom CSS for headings, cards, colors

Minimalistic, professional interface

Hoverable charts with smooth animations

Wide layout for better analytics experience

📝 Future Improvements

Daily portfolio history saving

Integration with real trading APIs

Advanced analytics (volatility, Sharpe ratio)

Dark mode

Sector analysis

Push notifications for price alerts

🤝 Contributing

Contributions are welcome!

Fork the repository

Create a feature branch

Commit changes

Open a pull request

📄 License

This project is free for personal and educational use.

🙏 Acknowledgments

Streamlit for UI components

yFinance for market data

Plotly for stunning visualizations

Pandas/NumPy for data processing

📈 Advanced Stock Portfolio Tracker

Smart investing starts with smart tracking.


