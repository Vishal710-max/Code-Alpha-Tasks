# Task Automation — Three-in-One Utility

A small, user-friendly command-line utility that bundles three common automation tasks into a single script with an improved UX (uses optional `rich` formatting when available):

- Move image files (JPG / JPEG / PNG) between folders with safe handling for cloud-backed files
- Extract email addresses from a text file and save them to an output file
- Scrape a webpage to extract title, meta description, and basic technical details and save them to a text file

The script is located at `task_automation.py`. The folder also includes a `requirements.txt` listing the main dependencies.

---

## Quick Start

1. Clone the repository (or download the `Task Automation` folder).
2. (Optional but recommended) Create a virtual environment:

   python -m venv .venv
   source .venv/bin/activate   # macOS / Linux
   .venv\Scripts\activate      # Windows

3. Install dependencies:

   pip install -r "Task Automation/requirements.txt"

   The requirements include:
   - rich (optional, for better visuals)
   - requests
   - beautifulsoup4

4. Run the script:

   python "Task Automation/task_automation.py"

---

## Usage Overview

When you run the script you'll see a simple menu with four options:

1. Move Image Files
   - Prompts for a source directory and destination directory.
   - Moves files with extensions `.jpg`, `.jpeg`, `.png`.
   - Performs safe moves and attempts to work around cloud file provider issues (e.g., OneDrive) using a copy+delete fallback.
   - Handles duplicate filenames by appending a counter.

2. Extract Email Addresses
   - Prompts for an input text file (a sample `sample_emails.txt` will be created if none is found).
   - Extracts email addresses using a regex, removes duplicates while preserving order, and saves results to `extracted_emails.txt` (or a file you specify).
   - Output includes a small header with source and timestamp.

3. Scrape Webpage Title
   - Lets you choose a test URL or enter a custom URL.
   - Uses `requests` + `beautifulsoup4` to fetch page title, meta description, keywords, and basic HTTP info.
   - Saves results to a timestamped text file `webpage_<domain>_<timestamp>.txt`.

4. Exit
   - Exits the program.

---

## Notes & Tips

- For best visuals, install `rich`: pip install rich
- If `beautifulsoup4` is missing, Task 3 will prompt you to install it: pip install beautifulsoup4
- If you get cloud/OneDrive-related errors when moving files, try:
  - Disabling OneDrive sync temporarily
  - Copying files to a local folder first
  - Running the script with elevated permissions if needed
- Network timeouts or connection errors may occur during web scraping; ensure you have internet access and the target site allows scraping.

---

## Troubleshooting

- PermissionError while moving files: try running the script with appropriate permissions, or ensure the file is not locked by another app.
- Cloud file provider errors: the script attempts a copy+delete fallback, but you may need to sync the files locally or disable the provider temporarily.
- BeautifulSoup import error: pip install beautifulsoup4
- Slow or failing web requests: try a different URL or increase network reliability.

---

## Contributing

Small improvements, bug fixes, or UX tweaks are welcome. Please open an issue or submit a pull request with a clear description of the change.

---

## License

MIT — feel free to use and adapt this script for your own needs.

---

## Author / Contact

Created by Vishal710-max (as part of Code-Alpha-Tasks)

Repository: https://github.com/Vishal710-max/Code-Alpha-Tasks
