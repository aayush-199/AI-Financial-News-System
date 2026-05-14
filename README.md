# AI-Financial-News-System
This project is an AI-powered financial news automation system built in n8n.  It automatically collects the latest financial news, analyzes it using AI, and sends clean professional news alerts directly to Telegram.
This project is an AI-powered financial news automation system built in n8n. It automatically collects the latest financial news, processes it using AI, and sends summarized market insights directly to Telegram. The goal of this system is to save traders time and quickly highlight important macro and market-moving events.

Schedule Trigger
This node automatically starts the workflow at a specific time interval. It acts like the system’s timer and checks for new financial news regularly.
HTTP Request
This node fetches live financial news data from a news source using an API or RSS feed link. It pulls the latest headlines and article information into the workflow.
XML
The fetched news data comes in XML format, which is difficult to use directly. This node converts the XML data into JSON format so the workflow can process it easily.
Edit Fields
This node cleans and organizes the important data from the news feed. It selects useful fields like title, link, and publish date while removing unnecessary information.
Basic LLM Chain
This is the AI brain of the project. It analyzes the financial news using a Groq AI model and generates simplified market insights such as sentiment, macro narrative, market bias, affected assets, and possible trade ideas.
Groq Chat Model
This node connects the workflow to Groq’s AI model. It powers the AI analysis and generates fast responses for the financial news summaries.
Send a Text Message
This node sends the final AI-generated news summary directly to a Telegram chat or channel. It allows the user to receive automated market updates instantly on Telegram.

Main Use Case:

This system helps forex, crypto, and stock traders quickly understand important market news without reading long articles manually. It acts like a personal AI macro news assistant that works automatically in the background.
