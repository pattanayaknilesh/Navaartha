# 🛒 Navaartha – AI-Powered Autonomous Dropshipping Agent 🤖📦

**Navaartha** (*Sanskrit: "new meaning"*) is a fully autonomous, AI-powered dropshipping agent that discovers trending products, finds low-cost suppliers, conducts competitive analysis, posts listings across multiple platforms, and manages order fulfillment — all with minimal human intervention.

Built at the intersection of commerce and intelligence, Navaartha aims to redefine digital retail with automation and scale.

---

## ⚙️ Features

### 🔍 Phase 1: Product Discovery & Sourcing
- Scrapes trending products from Reddit, Amazon, Google Trends, and niche blogs.
- Uses NLP and sentiment analysis to determine genuine user interest.
- Finds low-cost suppliers on platforms like AliExpress and Alibaba.
- Matches images via computer vision to ensure product accuracy.

### 📊 Phase 2: Competitive Analysis & Product Listing
- Analyzes pricing across major e-commerce sites (Amazon, eBay, Etsy, etc.).
- Dynamically sets competitive prices with target margin controls.
- Auto-generates SEO-optimized product titles and descriptions using GPT APIs.
- Posts listings via platform APIs (Amazon SP-API, eBay API, Shopify, etc.).

### 📦 Phase 3: Order Fulfillment & Logistics
- Monitors incoming orders across platforms.
- Orders are automatically placed with suppliers via APIs or automation.
- Integrates with Shiprocket API for shipment handling.
- Sends tracking updates to customers and platforms.

---

## 🧠 Tech Stack

- **Languages**: Python (core), JavaScript (dashboard/front-end)
- **AI Models**: OpenAI GPT, Hugging Face Transformers, custom-trained models
- **Scraping**: Scrapy, Playwright, BeautifulSoup
- **NLP**: spaCy, NLTK, Transformers
- **Vision**: OpenCV, CLIP (for image matching)
- **APIs**:
  - Reddit API, Google Trends, Amazon SP-API, eBay API, Shopify API
  - Shiprocket API (for shipping)
- **Automation**: Selenium / Puppeteer (for supplier sites without APIs)
- **Data**: PostgreSQL / MongoDB for product and order metadata
- **Frontend** (optional): React + TailwindCSS for dashboard & insights

---

## 🏗️ Project Structure

```bash
navaartha/
├── product_discovery/
│   ├── reddit_scraper.py
│   ├── trend_analyzer.py
│   └── google_trends.py
├── sourcing/
│   ├── supplier_scraper.py
│   ├── image_matcher.py
│   └── product_matcher.py
├── listing_engine/
│   ├── competitor_analysis.py
│   ├── price_optimizer.py
│   ├── content_generator.py
│   └── api_integrations/
├── fulfillment/
│   ├── order_monitor.py
│   ├── supplier_ordering.py
│   └── shiprocket_integration.py
├── utils/
│   ├── config.py
│   └── logger.py
└── README.md
