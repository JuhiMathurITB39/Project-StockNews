# Project-StockNews

Automate stock market news analysis and alerts using Python.
This bot fetches the latest stock market news, analyzes sentiment, and sends alerts to keep you updated on market trends.

Features
Fetches real-time stock market news from APIs
Analyzes sentiment (positive, negative, neutral) using NLP
Sends email or Telegram alerts for significant news
Customizable stock symbols and news sources
Simple setup with API key authentication


Project Structure
stock-news-bot/
│-- stock_news.py          # Main script for fetching and analyzing news
│-- requirements.txt       # Dependencies
│-- .gitignore             # Prevents sensitive files from uploading
│-- README.md              # Project documentation
│-- .env (Do NOT upload)   # Stores API keys and credentials
Installation & Setup
1. Clone the Repository
git clone https://github.com/JuhiMathurITB39/Project-StockNews
cd stock-news-bot

2. Install Dependencies
Make sure you have Python 3.8+ installed, then run:
pip install -r requirements.txt

3. Set Up Environment Variables
Create a .env file inside the project folder and add your API keys and email credentials:
STOCK_API_KEY=your-stock-api-key  
NEWS_API_KEY=your-news-api-key  
EMAIL_USER=your-email@example.com  
EMAIL_PASSWORD=your-email-password  
TELEGRAM_BOT_TOKEN=your-telegram-bot-token  
TELEGRAM_CHAT_ID=your-telegram-chat-id

4. Run the Bot
python stock_news.py

How It Works
1. Fetches real-time news for specified stock symbols
2. Analyzes sentiment using NLP
3. Filters high-impact news and summarizes key points
4. Sends email or Telegram alerts for important updates

Notes
Customization: Modify stock_news.py to change stock symbols, news sources, or sentiment thresholds.
Rate Limits: Check API rate limits to avoid hitting request limits.
Security: Do not upload .env files containing API keys.
Troubleshooting
API requests failing? Check if API keys are valid.
Emails not sending? Ensure you’ve enabled less secure apps (for Gmail) or use an SMTP relay.
Telegram alerts not working? Verify bot permissions and chat ID.
