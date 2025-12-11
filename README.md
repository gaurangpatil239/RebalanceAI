     
##         
RebalanceAI – Intelligent Portfolio Rebalancing Agent 
Overview 
RebalanceAI is an AI-powered financial analysis assistant that automates portfolio 
rebalancing, sentiment evaluation, and predictive investment recommendations using real
time market data. 
It leverages AI inference, predictive modeling, and financial data APIs (Yahoo Finance) to 
analyze top-performing stocks, visualize key trends, and provide actionable investment 
advice — all within a user-friendly Python interface. 
##         
Project Architecture 
**Pipeline Flow (End-to-End):** 
1. Data Fetching: Automatically retrieves top-performing stock data using yFinance API. 
2. Preprocessing: Cleans and structures stock metrics (open, close, volume, etc.). 
3. Visualization: Generates comparative charts and trends using Matplotlib and Plotly. 
4. Predictive Analysis: Computes EMA (Exponential Moving Average) and SMA (Simple 
Moving Average) for performance forecasting. 
5. AI Sentiment Analysis: Reads the generated charts and interprets market signals using 
OpenAI GPT-based models. 
6. Recommendation Engine: Suggests the best stock to rebalance/add to the user’s portfolio. 
7. Frontend Visualization (Optional): Displays charts and insights via an integrated 
Streamlit or Flask-based UI. 
##       
Key Features 
Automated Data Retrieval – Fetches top stocks dynamically from Yahoo Finance without 
manual input.   
Predictive Insights – Uses EMA and SMA for trend forecasting and momentum detection.   
AI Sentiment Recommendation – Generates human-readable investment 
recommendations.   
Data Visualization – Displays clear charts comparing stock performance.   
Modular Design – Separated backend (AI + data processing) and frontend (visual 
dashboard).   
Command-Line / App Execution – Launchable directly via terminal using:   
`python rebalanceai.py` 
##         
Tech Stack 
| Category | Tools & Libraries | 
|-----------|-------------------| 
| Programming Language | Python 3.9+ | 
| Data Fetching | yfinance, pandas, numpy | 
| Visualization | matplotlib, plotly, seaborn | 
| AI & NLP | openai, langchain | 
| Frontend (Optional) | streamlit or flask | 
| Deployment | VS Code, Google Colab, CLI execution | 
##     
Installation & Setup 
1. Clone the Repository 
``` 
git clone https://github.com/<yourusername>/RebalanceAI.git 
cd RebalanceAI 
``` 
2. Create a Virtual Environment 
``` 
python -m venv venv 
source venv/bin/activate  # Mac/Linux 
venv\Scripts\activate   # Windows 
``` 
3. Install Dependencies 
``` 
pip install -r requirements.txt 
``` 
4. Set Up API Key   
Use your OpenAI API key as an environment variable or inside the code (not 
recommended). 
## ▶️ Usage 
Run the Application: 
``` 
python rebalanceai.py 
``` 
Output Includes: - Real-time comparative charts of top 5 stocks   - EMA/SMA-based trend predictions   - AI-generated recommendations like: 
> “Based on the predictive chart and EMA trend, JPM shows the highest growth potential. It 
is recommended to add this stock to your portfolio for optimal balance.” 
##    
Folder Structure 
RebalanceAI/ 
│ rebalanceai.py 
│ data/ 
│ charts/ 
│ frontend/ 
│ requirements.txt 
│ README.md 
│ utils/ 
##     
Future Enhancements - Integrate live market sentiment data via Twitter/Reddit APIs. - Enable user portfolio upload (.csv) for custom analysis. - Add risk assessment & volatility scoring. - Deploy as a cloud-based dashboard using AWS or Streamlit Cloud. - Introduce reinforcement learning for dynamic portfolio rebalancing. 
##    
Authors 
**Gaurang Kiran Patil**   
**Pooja Mishra**   
Data Analytics Engineering | Northeastern University   
patil.gauran@northeastern.edu | mishra.po@northeastern.edu 
