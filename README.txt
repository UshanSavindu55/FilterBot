# FilterBot

**FilterBot** is a tool that automates the filtering and deletion of unwanted emails using customizable rules.

---

## 🚀 Project Overview

FilterBot uses the IMAP protocol to connect to your email and fetch the most recent emails. It automates the deletion of unwanted spam emails by filtering out messages flagged by a keyword or pattern check. FilterBot improves your email management by auto-deleting flagged emails.

FilterBot is great to learn email automation as well as Python scripting and productivity tool development to increase efficiency and save time.

---

## ⚙️ Features

- Compatible with any email service that supports IMAP (Gmail, Outlook, etc.).

- Handles email parsing with proper encoding.

- Offers customizable lists to filter emails.

- Deletes flagged emails automatically.

- Protects sensitive information using environment variables.

- Clean architecture and structure suitable for unit and integration testing with CI/CD pipelines.

---

## 📋 Getting Started

### Prerequisites

- Python version 3.8 or newer.

- Gmail or Outlook account with IMAP access.

- Gmail app password with 2FA turned on.

### Installation

1. Clone the repo:

```bash

git clone https://github.com/yourusername/filterbot.git

cd filterbot

2. Create and activate a virtual environment:

```bash

python -m venv venv
source venv/bin/activate   # macOS/Linux
venv\Scripts\activate      # Windows

3. Install Dependancies

```bash

pip install -r requirements.txt

4. Create a .env file in the root directory with your credentials

EMAIL=your_email@example.com
PASSWORD=your_app_password


🛠️ Usage

Run the main script to start filtering:

python src/main.py

The script will connect to your inbox, scan recent emails, flag unwanted ones based on keywords, and delete them automatically.


⚙️ Configuration

Edit configs/keywords.json to customize which keywords trigger filtering. Example:

[
  "win",
  "free",
  "prize",
  "urgent",
  "lottery"
]

🧪 Testing

Run unit tests with:

python -m unittest discover tests


📈 Future Improvements

- Integrate machine learning for smarter spam detection

- Add OAuth2 authentication support

- Build a GUI or web dashboard for easier interaction

- Schedule automatic runs with cron or Task Scheduler

- Add email backup before deletion

🤝 Contributing

Contributions and suggestions are welcome! Feel free to open issues or pull requests.