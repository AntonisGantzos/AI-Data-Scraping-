# AI Web Scraping with Ollama
# Project Overview
  This project demonstrates how to scrape data from websites, clean and structure the data, and use a Large Language Model (LLM), specifically the Ollama Llama3.1, to extract information from the text. The project automates the process of extracting structured data from unstructured web content and stores it in a CSV format.

# Key Features
  - Web Scraping: Uses Selenium and BeautifulSoup to scrape web pages and extract raw HTML content.
  - Data Cleaning: Strips unwanted elements such as scripts and styles using BeautifulSoup to retrieve clean, readable text.
  - Batch Processing: Divides large textual content into smaller batches to stay within the token limit of LLMs.
  - Information Extraction: Utilizes Ollama LLM (via LangChain) to extract specific structured data such as hurricane information.
  - CSV Export: Stores the extracted data into a CSV file for further analysis.

# Installation
  - Clone this repository: ```git clone <repository-url>```
  - Install the required packages: ```pip install -r requirements.txt```
  - Set up ngrok and authenticate your token: ```ngrok config add-authtoken <your-ngrok-auth-token>```
  - Install and configure the Ollama model: ```curl https://ollama.ai/install.sh | sh
ollama pull llama3.1```

# Customization
  You can modify the extraction criteria in the ```criteria``` variable to collect different kinds of data from the webpage. Additionally, the model can be fine-tuned for other tasks by adjusting the prompt template.

# Requirements
  - Python 3.x
  - Selenium
  - BeautifulSoup
  - Pyngrok
  - LangChain
  - Ollama LLM
  - Whisperx (optional)
