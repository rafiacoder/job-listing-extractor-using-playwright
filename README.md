# 🧠 Rozee.pk Job Listings Scraper (Playwright + Stealth Mode)

This project scrapes job listings from [Rozee.pk](https://www.rozee.pk) using **Playwright** in stealth mode.
It searches for a specific job title, city, and salary range, then extracts all available jobs with full details (title, company, location, link) — and saves them into a CSV file 
and handle pagination if there successfully

---

## 📂 Project Structure

```bash
job_listing_scraper/
│
├── main.py                # Entry point: runs automation + scraping
├── automation.py          # Applies search filters (title, city, salary)
├── job_listing_scraper.py # Extracts job listings, opens details, paginates,and save to csv
├── browser_config.py      # Creates stealth browser context
└── output/
    └── jobs_extracted_data.csv  # Saved job listings
🚀 How It Works
Launches Chromium browser in stealth mode

Fills out search filters:

Job Title: Python Developer
City: Lahore
Min. Salary: 8,000
Scrapes all job listings from search results
Opens each job in new tab to extract:
✅ Title

✅ Company

✅ Location

✅ Job Link

Handles pagination
Saves everything to a CSV file

🧭 My Journey to This Project

I initially built this automation using Selenium, and it worked well for basic interactions.
However, when I reached the scraping stage, I discovered that heavy JavaScript rendering on Rozee.pk required a more advanced tool.
That's when I switched to Playwright, and began learning it from scratch — exploring everything from sync vs async models to stealth techniques for bypassing bot detection.
I implemented this entire project using async Playwright, with a modular and scalable architecture.

👉 This shift not only improved scraping performance, but also gave me deeper insight into real-world automation and scraping challenges.
