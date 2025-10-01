# 📧 Email Scraper

A lightweight Python-based web crawler that extracts email addresses from a target website.  
It uses `requests` and `BeautifulSoup` to crawl links and a regex filter to collect emails.

---
## ✨ Features
- Crawl a target domain up to 100 pages (configurable in code).
- Extract and print email addresses found in the HTML.
- Automatically follows internal links.
- Simple and easy-to-use CLI tool.
---
## 🛠️ Requirements
- Python 3.7+
- Install dependencies:
```bash
pip install -r requirements.txt
```
- requirements.txt -
```bash 
beautifulsoup4
requests
lxml
```
---
## 🚀 Usage
1. Clone this repository:
```bash
git clone https://github.com/yourusername/email-scraper.git
cd email-scraper
```
2. Run the script:
```bash
python email-scarper.py
```

3. Enter the target URL when prompted:
```bash
[+] Enter Target URL To Scan: https://example.com
```
---
## 📂 Example Output
```bash
[1] Processing https://example.com
[2] Processing https://example.com/contact
[3] Processing https://example.com/about
contact@example.com
support@example.com
info@example.com
```
---
## ⚠️ Notes

- The script currently stops after processing 100 URLs (you can adjust if count == 100 in the code).
- It only scrapes publicly visible emails in page content; it does not bypass protections or scrape JavaScript-rendered data.
- Be mindful of crawling large websites.

---
## 📌 Future Improvements

- Add option to set crawl depth and page limit from CLI.
- Export results to a file (.txt or .csv).
- Detect obfuscated emails (e.g., user [at] domain [dot] com).

---
## 🤝 Contributing
Pull requests are welcome! For major changes, please open an issue first to discuss what you’d like to improve.

---
## 📜 License

MIT License. (@immortal)

