# Stock Market Monitoring with Twilio and Alpha Vantage API

This Python script monitors the stock market using the Alpha Vantage API to retrieve stock prices and the News API to fetch relevant news articles. If the percentage difference between yesterday's and the day before yesterday's closing stock prices exceeds 1%, it sends the top three news articles related to the specified stock via Twilio SMS.

## Features

- **Stock Price Monitoring**: Retrieves daily stock prices for the specified stock (e.g., TSLA - Tesla Inc) using the Alpha Vantage API.
- **News Article Retrieval**: Fetches news articles related to the specified stock using the News API.
- **Twilio Integration**: Sends the top three news articles as separate SMS messages via Twilio.
- **Customizable Parameters**: Allows customization of parameters such as the stock name, Twilio credentials, and API keys.

## How It Works

The script performs the following functions:

1. **Stock Price Retrieval**: Retrieves yesterday's and the day before yesterday's closing stock prices for the specified stock using the Alpha Vantage API.
2. **Percentage Difference Calculation**: Calculates the percentage difference between yesterday's and the day before yesterday's closing stock prices.
3. **News Article Retrieval**: If the percentage difference exceeds 1%, fetches news articles related to the specified stock using the News API.
4. **Message Formatting**: Formats the retrieved news articles and stock price difference as SMS messages.
5. **Twilio Integration**: Sends each formatted article as a separate SMS message via Twilio using the specified Twilio credentials.

## Usage

1. Ensure you have valid API keys for the Alpha Vantage API and the News API.
2. Configure the script with your Twilio account SID, auth token, virtual Twilio number, and verified phone number.
3. Set the desired stock name and company name.
4. Run the script using a Python interpreter.
5. Monitor your phone for SMS messages containing relevant news articles whenever significant changes in stock prices occur.

## Customization

You can customize the following aspects of the script:

- **Stock Name**: Modify the `STOCK_NAME` variable to specify the stock symbol you want to monitor.
- **Company Name**: Modify the `COMPANY_NAME` variable to specify the name of the company associated with the stock.
- **API Keys**: Replace the placeholder API keys (`STOCK_API_KEY` and `NEWS_API_KEY`) with your own API keys from Alpha Vantage and News API, respectively.
- **Twilio Credentials**: Replace the placeholder Twilio account SID (`TWILIO_SID`), auth token (`TWILIO_AUTH_TOKEN`), virtual Twilio number (`VIRTUAL_TWILIO_NUMBER`), and verified phone number (`VERIFIED_NUMBER`) with your own credentials.

## Prerequisites

Before running the script, ensure you have Python installed on your system. Additionally, sign up for accounts with Alpha Vantage, News API, and Twilio to obtain the necessary API keys and credentials.

