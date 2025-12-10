# Code-Alpha-Tasks

A small repository that collects three beginner-friendly Python projects. Each project is self-contained and demonstrates core programming concepts with simple, practical tasks you can run locally.

Projects included
- TASK 2 — Stock Portfolio Tracker
- TASK 3 — Task Automation with Python Scripts
- TASK 4 — Basic Chatbot

---

## Quick setup (create repo & push)
1. Create a new GitHub repository named `Code-Alpha-Tasks`.
2. Locally:
   ```bash
   mkdir Code-Alpha-Tasks
   cd Code-Alpha-Tasks
   git init
   ```
3. Add files and folders for each project (examples below).
4. Commit and push:
   ```bash
   git add .
   git commit -m "Initial commit: add 3 projects (Task 2, 3, 4)"
   git branch -M main
   git remote add origin https://github.com/<your-username>/Code-Alpha-Tasks.git
   git push -u origin main
   ```

---

## Recommended repository structure
Organize each task in its own folder:

Code-Alpha-Tasks/
- TASK-2-Stock-Portfolio-Tracker/
  - main.py
  - README.md
  - requirements.txt  
- TASK-3-Task-Automation/
  - task_automation.py
  - README.md
- TASK-4-Basic-Chatbot/
  - chatbot.py
  - README.md
- README.md (this file)

---

## TASK 2 — Stock Portfolio Tracker (simple)
Goal: Build a simple stock tracker that computes the total investment using manually defined stock prices.

What it does
- Accepts user input for stock symbol and quantity.
- Uses a hardcoded dictionary of prices, e.g.:
  ```python
  PRICES = {"AAPL": 180, "TSLA": 250, "MSFT": 300}
  ```
- Calculates and prints total value for each input and grand total.
- Optionally saves results to `portfolio.txt` or `portfolio.csv`.

How to run (example)
1. Create `main.py` inside `TASK-2-Stock-Portfolio-Tracker/`.
2. Run:
   ```bash
   python  main.py
   ```
3. Follow on-screen prompts (enter symbol and quantity). The script displays totals and can write to a file.

Key concepts: dictionaries, input/output, arithmetic, optional file handling.


---

## TASK 3 — Task Automation with Python Scripts
Goal: Automate small, real-life repetitive tasks.  

Suggested scripts
- move all `.jpg` files from source folder to a target folder (uses `os`, `shutil`)
- read a `.txt` file and extract emails into another file (uses `re`)
- fetch a fixed webpage and save its `<title>` (uses `requests`, `bs4` or `re`)

How to run
```bash
python move_images.py src_folder dest_folder
python extract_emails.py input.txt output_emails.txt
python scrape_title.py https://example.com title.txt
```

Key concepts: os, shutil, re, requests, file handling.

---

## TASK 4 — Basic Chatbot
Goal: Build a small rule-based chatbot that responds to a few user inputs.

Behavior
- Recognizes simple inputs like: "hello", "how are you", "bye"
- Replies with predefined outputs: "Hi!", "I'm fine, thanks!", "Goodbye!"
- Runs a loop until user says "bye"

How to run
1. Create `chatbot.py` inside `TASK-4-Basic-Chatbot/`.
2. Run:
   ```bash
   python chatbot.py
   ```
3. Chat via the terminal.

Key concepts: conditional statements (if/elif), functions, loops, user input/output.

---

## Contributing
- Fork the repo, add or improve project code, then open a pull request.
- Keep changes small and describe how to run your code.

---

## License
Use freely for personal and educational purposes.

---
