ProjexFX - MT4/MT5 FX Signal Copy trading Telegram Bot!
This Telegram bot lets you enter trades directly from Telegram and view the risk-to-reward ratio, profit, loss, and calculated lot size. You can adjust settings like allowed symbols and risk factor via a personalized Python script and environment variables.

Features
Copy Trades: Directly from signal providers or personal analysis.
Account Info: Retrieve MT4/MT5 account info (balance, equity, open positions, etc.) via MetaAPI.
Order Types: Place all 6 order types (Market Buy/Sell, Limit Buy/Sell, Buy/Sell Stop) from Telegram.
Risk-to-Reward Calculation: Using stop loss and take profit, displays size in pips and profit/loss (USD).
Multiple Take Profits: Place up to two take profits using half position size for each.
Future Feature: Trailing stop loss

1. Installation
Prerequisites:

Telegram Account
MetaAPI Account (Sign Up)
Render Account (Sign Up)
Steps:


2. Create a Telegram Bot:

Talk to @BotFather on Telegram to create a new bot and save the API token.
Set Up on Render:

Go to your Render dashboard and create a new web service application.
Use this public Git repository URL: https://github.com/ogunjobiFX/MT4-MT5-Forex-Signal-Copier-Telegram-Bot
Configure Render Application:

Name your application (e.g., mt4tradingbot).
Set the build command: pip install -r requirements.txt
Set the start command: python run.py
Create the web service.
Set Up Environment Variables:

Navigate to the environment tab in your Render dashboard and set the following variables:
arduino
Copy code
Key             Value
PYTHON_VERSION  3.8.2
TOKEN           "INSERT TELEGRAM BOT API TOKEN HERE"
APP_URL         "https://[INSERT NAME OF APP HERE].onrender.com/"
TELEGRAM_USER   "INSERT TELEGRAM USERNAME HERE"
API_KEY         "INSERT META API TOKEN HERE" (https://app.metaapi.cloud/token)
ACCOUNT_ID      "INSERT META API ACCOUNT ID HERE" (https://app.metaapi.cloud/accounts)
RISK_FACTOR     "INSERT PERCENTAGE OF RISK PER TRADE HERE IN DECIMAL FORM, e.g., 5% = 0.05"
Deploy:

Check the events tab for deployment logs. If there are no errors, your bot is running.
Edit Environment Variables:

Make changes via the Render web app. The app will redeploy automatically with new changes.
Congratulations! 

*You can now open a conversation with your bot on Telegram. Send the /help command for instructions and example trades.*






