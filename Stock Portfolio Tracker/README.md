# Advanced Stock Portfolio Tracker

📈 Smart, simple, and analytics-driven stock portfolio manager built with Python and Streamlit.

A lightweight Streamlit app to track holdings, view real-time prices (via yFinance), analyze portfolio performance, and export data. Designed for personal use, learning, and small-scale portfolio monitoring.

---

## Table of contents
- [Features](#features)
- [Demo / Screenshots](#demo--screenshots)
- [Tech stack](#tech-stack)
- [Requirements](#requirements)
- [Install & Run](#install--run)
- [Quick start](#quick-start)
- [Usage](#usage)
- [Project structure](#project-structure)
- [Data & reliability notes](#data--reliability-notes)
- [Development](#development)
- [Contributing](#contributing)
- [License & Acknowledgements](#license--acknowledgements)
- [Contact](#contact)

---

## Features
- Real-time price lookup using yFinance
- Auto-calculated portfolio metrics: total value, cost basis, gain/loss (amount and %)
- Add / remove (sell) holdings; supports partial sells and automatic average-price recalculation
- Transaction history with timestamps and color-coded BUY/SELL entries
- Interactive charts:
  - Portfolio value over selectable ranges (1W, 1M, 3M, 6M, 1Y, All)
  - Allocation donut chart
  - Gain/Loss comparison bar chart
- Export portfolio and transactions to CSV or JSON
- Clean Streamlit layout with Plotly charts and custom styling

---

## Demo / Screenshots
(Replace these with actual screenshots in the repo)
- Overview dashboard with portfolio value chart
- Holdings table with current value and gain %
- Transaction history and export panel

---

## Tech stack
- Frontend: Streamlit
- Language: Python 3.8+
- Charts: Plotly (graph_objects / express)
- Data: yFinance
- Data handling: pandas, numpy
- Session storage: Streamlit session_state

---

## Requirements
- Python 3.8 or higher
- Internet connection (for fetching live prices)

Install dependencies:
```bash
pip install -r requirements.txt
```

---

## Install & Run
1. Clone the repo:
```bash
git clone https://github.com/Vishal710-max/Code-Alpha-Tasks.git
cd "Code-Alpha-Tasks/Stock Portfolio Tracker"
```

2. Install:
```bash
python -m venv .venv        # optional but recommended
source .venv/bin/activate   # or .venv\Scripts\activate on Windows
pip install -r requirements.txt
```

3. Run:
```bash
streamlit run main.py
```

Visit http://localhost:8501

---

## Quick start
- Add a new holding: enter symbol (e.g., AAPL), quantity, optional purchase price → Add to Portfolio
- Remove / Sell: choose a holding and quantity → Remove from Portfolio (partial sells supported)
- View charts: switch between Overview, Performance, Holdings, Transactions tabs in the sidebar
- Export: choose CSV or JSON and click Download

---

## Usage notes
- If purchase price is omitted, the app uses current market price as cost basis (you can adjust later)
- The app stores data in Streamlit's session_state for the current session — closing the browser or restarting the app will reset data unless you export it
- Exporting transaction history preserves timestamps and actions for audit

---

## Project structure
stock-portfolio-tracker/
- main.py               # Streamlit app entrypoint
- README.md             # This file
- requirements.txt      # Python dependencies
- src/                  # (optional) helper modules
- assets/               # (optional) images and CSS

Adjust paths according to existing repository layout.

---

## Data & reliability
- Uses yFinance for market data; service outages or network failures may cause temporary unavailability
- The app includes fallback handling for missing data where possible, and prevents invalid operations (e.g., removing more quantity than owned)
- Prices are real-time but not suitable for trading decisions — use official broker quotes for execution

---

## Development
- Recommended: create a feature branch for changes
- Add tests where appropriate
- Linting & formatting: use black / flake8 (optional)
- To add new features (e.g., persistent storage, trading API integration), follow the existing module structure and submit a PR

---

## Contributing
Contributions are welcome:
1. Fork the repository
2. Create a feature branch: git checkout -b feature/your-feature
3. Commit changes and open a pull request
4. Provide clear description and testing instructions

Please include descriptive commit messages and small focused PRs for faster review.

---

## License & Acknowledgements
- This project is free for personal and educational use.
- Acknowledgements:
  - Streamlit — UI framework
  - yFinance — market data
  - Plotly — visualizations
  - pandas / NumPy — data processing

---

## Contact
Created by Vishal (Vishal710-max). For questions or suggestions, open an issue or a pull request in this repo.

Smart investing starts with smart tracking — enjoy!
