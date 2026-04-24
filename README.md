<img width="500" height="600" alt="image" src="https://github.com/user-attachments/assets/f2a4df44-3765-4641-b4f7-170929353bc1" />

<img width="600" height="950" alt="Screenshot 2026-04-24 165955" src="https://github.com/user-attachments/assets/4463943f-3238-4099-9871-10d7b2053b36" />

1. AI Shopping Assistant Overview
1.1 Traditional Online Shopping Challenges
Traditional online shopping can be a time-consuming and frustrating experience for users. Common problems include:

Too Many Results: Hundreds of results appear, overwhelming the user.
Time-Consuming: Users spend excessive time comparing prices and features across multiple products.
Lack of Personalization: Shoppers do not receive personalized recommendations or styling advice.
As a result, users spend more time searching for products than actually shopping, leading to frustration.

1.2 The AI Shopping Assistant Solution
The AI Shopping Assistant on Telegram offers the following features to overcome these challenges:

Text-based Product Search: Users can type their product requests and receive instant results.
Voice Message Support: Users can speak their queries instead of typing them.
Real-Time Amazon Scraping: The assistant fetches live data from Amazon, including product prices and ratings.
Personalized Styling Recommendations: The assistant provides tailored fashion advice based on user preferences.
Key Benefits:

No need to open websites or apps—everything happens inside Telegram.
Instant responses with the top 5 most relevant products.
Personalized fashion recommendations powered by AI.
In this session, we will focus on building AI shopping assistant with text based product search feature

1.3 Building the Shopping Assistant
Let's build shopping assistant by following the below steps

Configuring Telegram Bot

Adding AI Agent

Searching for Products

Sending Response Back to Telegram

Step 1: Configuring Telegram Bot
To create the Telegram bot, we use BotFather on Telegram

Telegram Integration with N8N: Use the Telegram node in N8N to set up a trigger that listens for messages from users and activates the workflow whenever a message is received.

Steps to configure telegram bot
Step 2: Adding an AI Agent
Integrate AI Model: Use AI models like Google Gemini or Claude to process the user’s query (e.g., "red dress under 2000") and return relevant product results.
Step 3: Searching for Products
When users ask for products like "red shirt under 2000", we need to Search Amazon India in real-time, Get actual product names, prices, and ratings and Show only relevant results

Scraper API: The Scraper API allows you to fetch live product data from Amazon. This helps in scraping product names, prices, ratings, and other relevant details in real time.

Using the HTTP Request Tool in N8N: This tool connects to the Scraper API, sending requests to fetch product data from Amazon and then returning this data to the workflow.

Set System Instructions: Configure the AI agent to process the user query and generate appropriate responses.
