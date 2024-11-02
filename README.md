# 📧 Cold Email Generator

The **Cold Email Generator** is a powerful application that automatically generates cold emails tailored to potential clients based on job postings. Built with [Streamlit](https://streamlit.io/) and [LangChain](https://python.langchain.com/), this tool extracts job information from URLs and uses your specified portfolio of projects to create relevant, impactful cold emails.

## 🎯 Features
- **Job Information Extraction**: Scrapes job posting information from a given URL.
- **Portfolio Matching**: Matches relevant projects from your portfolio to highlight specific skills.
- **Automated Email Generation**: Creates a personalized email in seconds, ready to send to potential clients.

## 🛠️ Setup & Installation

1. **Clone the Repository**
   ```bash
   git clone https://github.com/your-username/cold-email-generator.git
   cd cold-email-generator
2. Install Dependencies Make sure you have Python 3.7+ installed, then install the required packages:
 pip install -r requirements.txt
3. Configure Environment Variables
 GROQ_API_KEY=your_actual_api_key

4. Prepare Portfolio Data
  Add your portfolio projects in the my_portfolio.csv file located at app/resource/.
  The CSV file should have the following columns


Techstack,Links
Python; AI; Machine Learning,http://link-to-project.com

## 🚀 Running the Application
streamlit run main.py

Once the app is running, open http://localhost:8501 in your browser.

## 📜 Usage Guide
1. Enter the Job URL: Paste the URL of a job posting in the input field.
2. Submit the URL: Click the Submit button to start the job extraction and email generation.
3. View Generated Email: The application will display a tailored email for the specified job posting. You can copy it directly or customize it further

## 📂 Project Structure
```plaintext
cold-email-generator/
│
├── chains.py                # Contains the Chain class for job extraction and email generation.
├── main.py                  # Main Streamlit application file.
├── portfolio.py             # Manages the portfolio projects and their retrieval.
├── utils.py                 # Helper functions (e.g., for text cleaning).
├── .env                     # Environment variables (GROQ_API_KEY).
├── requirements.txt         # Python package dependencies.
└── README.md                # Project documentation.
```
## 🐛 Troubleshooting
Invalid API Key: Ensure the GROQ_API_KEY in your .env file is correctly formatted. Try using the API key directly in chains.py if issues persist.
Environment Variable Not Loaded: Make sure .env is in the project root. Alternatively, specify the full path to .env in load_dotenv().

### 👥 Contributing
1. Fork this repository.
2. Create a new branch with your feature: git checkout -b my-feature
3. Commit your changes: git commit -am 'Add new feature'
4. Push to the branch: git push origin my-feature
5. Create a pull request.
