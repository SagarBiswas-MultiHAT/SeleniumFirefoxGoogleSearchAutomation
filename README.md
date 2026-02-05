
# Selenium Google Search Automation

A simple script to automate web interactions using Selenium. This script demonstrates opening a Firefox browser, navigating to Google, and performing a search query.

## Features

- Opens Firefox browser.
- Navigates to Google.
- Searches for "Hello, Google!".
- Displays search results.

## Requirements

- Python 3.x
- Selenium

## Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/SagarBiswas-MultiHAT/selenium-google-search-automation.git
   ```
2. Navigate to the project directory:
   ```bash
   cd selenium-google-search-automation
   ```
3. Install Selenium:
   ```bash
   python -m venv .venv
   .\.venv\Scripts\Activate.ps1

   pip install selenium
   ```

## Usage

1. Run the script:
   ```bash
   python script.py
   ```

---

## Future Improvements (Recommended & Ethical)

✅ CAPTCHA-Safe & Legal Approach

### Google Custom Search JSON API (Official)

Link: https://console.cloud.google.com/

Why this matters

- Zero CAPTCHA
- No IP bans
- Fully legal
- Interview-safe
- Production-grade

🔹 Free Tier

- 100 searches/day — FREE
- Credit card required for activation

🔹 Pros

- Official Google API
- Stable & predictable
- Ideal for portfolios and demos
- No browser automation required

🔹 Cons

- Requires API key + Custom Search Engine (CSE)
- Paid after free quota (~$5 per 1,000 searches)

🏆 Verdict

Best option for:

- Clean engineering
- Legal compliance
- Long-term reliability
- Professional projects

---

What you’ll get at the end

You will have two things (both required):

- **API Key** (from Google Cloud)
- **Search Engine ID (CX)** (from Google Custom Search)

Only when you have both does the API work.

STEP 1 — Create a Google Cloud project

1. Open: https://console.cloud.google.com/
2. Log in with your Google account
3. At the top bar → click **Select a project**
4. Click **NEW PROJECT**
5. Set:

   - Project name: anything (e.g. `custom-search-api`)

6. Click **Create**

📌 This project will own your API key.

STEP 2 — Enable “Custom Search API”

1. Inside your project, go to: **APIs & Services → Library**
2. Search for **Custom Search API**
3. Click **Custom Search API**
4. Click **Enable**

✅ API is now active for your project.

STEP 3 — Create the API Key

1. Go to **APIs & Services → Credentials**
2. Click **Create Credentials**
3. Choose **API key**
4. Copy the key and save it somewhere safe

Example format:

`AIzaSyDxxxxxxxxxxxxxxxxxxxxxxx`

⚠️ Don’t share this publicly.

STEP 4 — Create a Custom Search Engine (CSE)

This is where many people get confused — follow exactly.

1. Open: https://programmablesearchengine.google.com/
2. Click **Add**
3. Fill the form:

   - Sites to search: Put `www.google.com` (temporary — we’ll change it)
   - Name: anything (e.g. `my-search-engine`)

4. Click **Create**

Now your search engine exists.

STEP 5 — Allow searching the entire web

By default, CSE only searches selected sites — we must change this.

1. On the CSE page → click **Edit**
2. Go to **Basics**
3. Find **Search the entire web**
4. Turn it **ON**
5. Save changes

✅ Now it behaves like Google Search.

STEP 6 — Get the Search Engine ID (CX)

1. In CSE settings → **Basics**
2. Copy **Search engine ID**

Example:

`a1b2c3d4e5f6g7h8i`

This is your CX value.

STEP 7 — Confirm your free quota

Google gives:

- ✅ 100 searches per day — FREE
- Paid after that (optional)

Check quota here:
Google Cloud Console → **APIs & Services → Quotas**

What you should now have

| Item | Example |
|------|---------|
| API Key | `AIzaSy...` |
| Search Engine ID (CX) | `a1b2c3...` |

If you have both, you’re ready.

Test URL (optional sanity check)

Paste this in your browser (replace values):

```
https://www.googleapis.com/customsearch/v1?key=API_KEY&cx=CX&q=hello+google
```

If it returns JSON → ✅ success

Feel free to contribute and enhance the script. Happy coding!
