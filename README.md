# URL Classification Web App 🛡️

A machine learning-powered web application built with Streamlit that classifies URLs into different threat categories using AI models.

## 🎯 Features

- **Real-time URL Analysis**: Classify URLs as Benign, Defacement, Phishing, or Malware
- **Multiple ML Models**: Choose between Random Forest and XGBoost classifiers
- **Interactive UI**: Clean, user-friendly interface with animated elements
- **Feature Extraction**: Comprehensive URL feature analysis including:
  - HTTPS detection
  - URL length and structure analysis
  - Special character counts
  - Geographic region detection
  - Shortening service detection
  - IP address detection
  - And more...

## �️ Installation

### Prerequisites
- Python 3.7 or higher
- Git with Git LFS installed (for large model files)

### Setup Instructions

1. **Clone the repository**
   ```bash
   git clone https://github.com/Jwongjs/Malicious-Webpage-URL-Detection_Streamlit.git
   cd Malicious-Webpage-URL-Detection_Streamlit
   ```

2. **Create a virtual environment**
   ```bash
   python -m venv .venv
   ```

3. **Activate the virtual environment**
   ```bash
   # Windows
   .venv\Scripts\activate
   
   # macOS/Linux
   source .venv/bin/activate
   ```

4. **Install dependencies**
   ```bash
   pip install -r requirements.txt
   ```

5. **Run the application**
   ```bash
   streamlit run mainPage.py
   ```

## 📁 Project Structure

```
├── mainPage.py                 # Main Streamlit application
├── feature_extraction_script.py # URL feature extraction logic
├── lottie_animations.py        # Animation handling
├── requirements.txt            # Python dependencies
├── Run_Instructions.txt        # Setup instructions
├── Models/
│   ├── rf_classifier.pkl       # Random Forest model (Git LFS)
│   └── xgboost_classifier.pkl  # XGBoost model (Git LFS)
├── lottie_animations/
│   └── mainpage.json          # Animation files
├── .gitattributes             # Git LFS configuration
├── .gitignore                 # Git ignore rules
└── README.md                  # Project documentation
```

## 🧠 Machine Learning Models

The application uses two pre-trained models:

- **Random Forest Classifier**: Ensemble learning method using multiple decision trees
- **XGBoost Classifier**: Gradient boosting framework optimized for performance

Both models classify URLs into four categories:
=======
Both models are trained to classify URLs into four categories:
- 🟢 **Benign**: Safe, legitimate websites
- 🟡 **Defacement**: Websites with unauthorized visual modifications
- 🔴 **Phishing**: Fake websites designed to steal information
- ⚫ **Malware**: URLs containing harmful software

## 🔍 URL Features Analyzed

| Feature Category | Features |
|------------------|----------|
| **Protocol Analysis** | HTTPS detection, abnormal URL patterns |
| **URL Structure** | Length, special characters (@,?,-,=,#,%,+,$,!,*,comma,//), letters, digits |
| **Domain Analysis** | Primary domain, secondary domain, geographic region |
| **Security Indicators** | IP addresses, URL shorteners, suspicious patterns |

## 🎮 Usage

1. **Select a Model**: Choose between Random Forest or XGBoost
2. **Enter URL**: Input the URL you want to analyze (must include http:// or https://)
3. **Click Analyze**: Press the "🔍 Check URL" button
4. **View Results**: See the classification result and detailed feature analysis

### Example URLs for Testing

Test the application with URLs from these sources:
- [PhishTank](https://phishtank.org/) - Known phishing URLs
- [URLhaus](https://urlhaus.abuse.ch/browse/) - Malware URLs
- [BadSSL](https://badssl.com/) - Various SSL/security test cases

## 🚀 Deployment

This app is configured for easy deployment on Streamlit Cloud with Git LFS support for large model files.

### Deploy to Streamlit Cloud

1. Push your repository to GitHub (with Git LFS configured)
2. Visit [share.streamlit.io](https://share.streamlit.io)
3. Connect your GitHub repository
4. Set the main file path to `mainPage.py`
5. Deploy!

## ⚠️ Disclaimer

This prediction tool is for educational and research purposes. The accuracy depends on the training dataset and should not be the sole factor in making security decisions. Always use multiple security tools and best practices when assessing URL safety.

## 🛠️ Technical Requirements

```
streamlit>=1.28.0
=======
The app extracts and analyzes multiple features from URLs:

| Feature Type | Description |
|--------------|-------------|
| **Protocol Analysis** | HTTPS vs HTTP detection |
| **URL Structure** | Length, special characters, digits, letters |
| **Domain Analysis** | Primary domain, secondary domain, geographic region |
| **Security Indicators** | IP addresses, URL shorteners, abnormal patterns |

## 📋 Requirements

```
streamlit
streamlit-lottie
tld
urllib3
numpy
<<<<<<< HEAD
scikit-learn
xgboost
tldextract
pandas
```

## 🤝 Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
=======
```

## 🎮 Usage

1. **Select a Model**: Choose between Random Forest or XGBoost
2. **Enter URL**: Input the URL you want to analyze
3. **Click Analyze**: Press the "🔍 Check URL" button
4. **View Results**: See the classification result and detailed analysis

### Example URLs for Testing

You can test the application with URLs from these sources:
- [PhishTank](https://phishtank.org/) - Known phishing URLs
- [URLhaus](https://urlhaus.abuse.ch/browse/) - Malware URLs
- [BadSSL](https://badssl.com/) - Various SSL/security test cases

## ⚠️ Disclaimer

This prediction tool is for educational and research purposes. The accuracy depends on the training dataset and should not be the sole factor in making security decisions. Always use multiple security tools and best practices when assessing URL safety.
>>>>>>> 99f9c4b9848a07046b290eddef976d5438dbb8af

## 🙏 Acknowledgments

- Built with [Streamlit](https://streamlit.io/)
- Animations powered by [Lottie](https://lottiefiles.com/)
- Machine learning models using [scikit-learn](https://scikit-learn.org/) and [XGBoost](https://xgboost.readthedocs.io/)
<<<<<<< HEAD
