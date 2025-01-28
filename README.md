
# Real-Time Competitor Strategy Tracker for E-Commerce

## Project Overview

This project is designed to help e-commerce businesses stay ahead of the competition by providing real-time insights into competitor pricing, discount strategies, and customer sentiment. By leveraging advanced machine learning techniques and natural language processing (NLP), this solution offers actionable data to improve strategic decision-making.

The system continuously monitors competitor activity, forecasts trends, and analyzes customer reviews to uncover insights that help businesses refine their strategies. Additionally, it integrates with Slack to send real-time notifications whenever significant changes in pricing, discounts, or customer sentiment are detected.

## Key Features

- **Competitor Data Aggregation**: Automatically collects and stores competitor data related to product prices and discount strategies over time.
- **Sentiment Analysis**: Utilizes Hugging Face Transformers to analyze customer reviews and extract actionable insights regarding product sentiment.
- **Predictive Modeling**: Implements ARIMA (AutoRegressive Integrated Moving Average) models to forecast competitor discounting strategies and price changes.
- **Slack Integration**: Sends real-time Slack notifications whenever significant changes in pricing or sentiment are detected, allowing businesses to take immediate action.
- **Interactive Dashboard**: Users can view competitor data, sentiment analysis results, and forecasts through an easy-to-use Streamlit app.

## Benefits

- **Real-Time Insights**: Monitor competitors in real time to adjust strategies quickly and stay ahead.
- **Enhanced Decision-Making**: Gain deeper insights into customer sentiment and competitor strategies, helping you make data-driven decisions.
- **Competitive Advantage**: By tracking competitor discounts and price changes, businesses can respond proactively to market shifts.
- **Easy Integration**: Streamlit app for easy deployment and integration with Slack for real-time updates.

## Technologies Used

- **Python**: Main programming language used for data analysis, machine learning, and app development.
- **Streamlit**: Framework for building interactive web applications, providing an intuitive dashboard.
- **Pandas**: Used for data manipulation, cleaning, and analysis of competitor and review data.
- **Hugging Face Transformers**: Pre-trained models used for performing sentiment analysis on customer reviews.
- **ARIMA**: A time series forecasting method used to predict future pricing and discount trends based on historical data.
- **Slack API**: Allows sending automated notifications to Slack channels about competitor activity and product changes.
- **BeautifulSoup & Requests**: Web scraping tools used for collecting competitor data from e-commerce websites.

## Setup Instructions

### 1. Clone the Repository
```bash
git clone <repository-url>
cd <repository-directory>
```

### 2. Install Dependencies
To install the required Python libraries, run the following command:
```bash
pip install -r requirements.txt
```

### 3. Configure API Keys
This project requires the following keys to function correctly:
- **Groq API Key**: For generating strategic recommendations based on competitor data.
   - Sign up for a Groq account at [Groq](https://groq.com).
   - Obtain your API key from the Groq dashboard.
   - Add the API key to the `app.py` file.

- **Slack Webhook URL**: For sending real-time notifications.
   - Go to the [Slack API](https://api.slack.com/apps), create a new app, and enable **Incoming Webhooks**.
   - Add a webhook to a Slack channel and copy the generated URL.
   - Paste the URL into the `app.py` file.

### 4. Run the Application
Start the application using Streamlit:
```bash
streamlit run app.py
```

The Streamlit app will open in your browser, where you can interact with the competitor strategy tracker.

### 5. Sample Data Files
This project includes sample data files for competitor analysis and sentiment analysis:
- **`competitor_data.csv`**: Contains product pricing, discounts, and dates of competitors.
- **`reviews.csv`**: Includes sample customer reviews for sentiment analysis.
- **`strategic_recommendations.csv`** (optional): Contains generated insights based on competitor pricing and sentiment.

## Usage

1. Launch the Streamlit app by running `streamlit run app.py`.
2. On the sidebar, select a product or competitor to analyze.
3. View detailed insights on competitor pricing, discount trends, and customer sentiment analysis.
4. Access predictive forecasts based on ARIMA modeling of competitor pricing and discounts.
5. Receive real-time Slack notifications about significant changes in competitor strategies and customer sentiment.
6. Use strategic recommendations to inform your own pricing and discount strategies.

## Project Files

- **`app.py`**: The main application script, implementing the core business logic, data analysis, and visualization.
- **`scrape.py`**: Web scraping script used to collect competitor pricing and discount data from e-commerce websites.
- **`competitor_data.csv`**: Sample data representing competitor products, their prices, and discounts.
- **`reviews.csv`**: Sample customer reviews used for sentiment analysis.
- **`requirements.txt`**: A list of required dependencies for the project.
- **`strategic_recommendations.csv`** (optional): Contains recommendations generated by analyzing competitor strategies and sentiment.

## Contributing

We welcome contributions to enhance the functionality of this project. To contribute:
1. Fork the repository.
2. Clone your fork to your local machine.
3. Create a new branch for your feature or bug fix.
4. Commit your changes and push to your fork.
5. Create a pull request.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
