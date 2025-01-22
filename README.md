# README: AI Travel Agent - Powered by LangGraph 🌍✈️  

## Overview  
The AI Travel Agent is a smart travel assistant leveraging LangGraph and multiple LLMs to streamline travel planning. It helps users find flights, book hotels, and send personalized travel plans via email, ensuring a seamless and interactive experience.

---

## Features  
- **Stateful Interactions**: Remembers user context for a smooth experience.  
- **Human-in-the-Loop**: Allows user control over critical actions like email review.  
- **Dynamic LLM Usage**: Adapts LLMs for tasks such as tool invocation and email generation.  
- **Email Automation**: Sends detailed travel plans directly to the user.  

---

## Installation  
1. Clone the repository:  
   ```bash
   git clone git@github.com:nirbar1985/ai-travel-agent.git  
   cd ai-travel-agent  
   ```  
2. Set Python version (if using pyenv):  
   ```bash
   pyenv local 3.11.9  
   ```  
3. Install dependencies:  
   ```bash
   poetry install --sync  
   poetry shell  
   ```  

---

## Setup API Keys  
1. Create a `.env` file in the project root.  
2. Add the following keys:  
   ```env
   OPENAI_API_KEY=your_openai_api_key  
   SERPAPI_API_KEY=your_serpapi_api_key  
   SENDGRID_API_KEY=your_sendgrid_api_key  
   LANGCHAIN_API_KEY=your_langchain_api_key  
   LANGCHAIN_TRACING_V2=true  
   LANGCHAIN_PROJECT=ai_travel_agent  
   ```  

Replace placeholders with your actual API keys.  

---

## Running the Chatbot  
1. Start the app:  
   ```bash
   streamlit run app.py  
   ```  
2. Enter your travel requests, e.g.:  
   *I want to travel to Amsterdam from Madrid from October 1st to 7th. Find me flights and 4-star hotels.*  

---

## Example Outputs  
- Flight and hotel options with logos and links.  
- Email integration with user control for customization.  

---

## Notes  
- Travel data fetched via Google Flights and Google Hotels APIs.  
- Results include links for easy navigation.  

Enjoy effortless travel planning with AI Travel Agent!
