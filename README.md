# AI-Legal-Sentiment-Analyzer

# ⚖️ Legal Document Sentiment Analysis

![Version](https://img.shields.io/badge/version-1.0-blue.svg)
![Python](https://img.shields.io/badge/python-3.8%2B-blue.svg)

## 📋 Overview

Legal Document Sentiment Analysis is an AI-powered tool designed to help legal professionals analyze documents for sentiment classification and risk assessment. Using advanced NLP models including RoBERTa and FinBERT, the application provides comprehensive analysis of legal texts to identify potential compliance issues, assess document sentiment, and generate risk reports.

## ✨ Features

- 🤖 **Advanced AI Models**: Utilizes RoBERTa and FinBERT for accurate sentiment analysis
- 📄 **Single Document Analysis**: Analyze individual legal documents with detailed insights
- 📊 **Batch Processing**: Process multiple documents simultaneously for comprehensive analysis
- ⚠️ **Risk Assessment**: Automated risk level classification (High/Medium/Low)
- 📈 **Interactive Visualizations**: Dynamic charts and graphs using Plotly
- 🎯 **Confidence Scoring**: Detailed confidence metrics for each analysis
- 📋 **Comprehensive Reports**: Generate detailed analysis summaries and recommendations
- 📱 **User-Friendly Interface**: Intuitive Gradio-based web interface

## 🔧 Installation

### Prerequisites
- Python 3.8 or higher
- pip package manager
- Internet connection for model downloads

### Quick Installation
```bash
# Clone the repository
git clone https://github.com/yourusername/legal-sentiment-analysis.git
cd legal-sentiment-analysis

# Install required packages
pip install -r requirements.txt

# Run the application
python app.py
```

### Manual Installation
```bash
# Install individual packages
pip install gradio
pip install transformers
pip install torch
pip install pandas
pip install numpy
pip install matplotlib
pip install seaborn
pip install plotly
```

## 🚀 How to Use

### Single Document Analysis
1. Launch the application by running `python app.py`
2. Open your browser and navigate to the provided local URL (typically `http://localhost:7860`)
3. Go to the "Single Document Analysis" tab
4. Paste your legal document text in the input field
5. Click "Analyze Document" to get instant results
6. Review the sentiment, confidence scores, and risk assessment

### Batch Document Analysis
1. Navigate to the "Batch Document Analysis" tab
2. Enter multiple documents separated by empty lines
3. Click "Analyze All Documents" for comprehensive batch processing
4. Review the summary statistics and detailed results table
5. Explore interactive visualizations for deeper insights

### Sample Documents
- Click "Load Sample Documents" to test the application with pre-loaded legal text examples

## 🖥️ Demo Screenshots
![Demo Interface]![image](https://github.com/user-attachments/assets/2ad80bd2-307b-4adb-89e3-585a275da251)


## 🚀 WorkFlow
```
Input Document → Text Preprocessing → AI Model Analysis → Risk Assessment → Visualization → Report Generation
```

![Workflow Diagram](https://via.placeholder.com/800x200/28a745/ffffff?text=Workflow+Diagram)
*Add your actual workflow diagram here*

## 🧠 How It Works

The Legal Document Sentiment Analysis tool employs a multi-model approach:

### 1. **Text Preprocessing**
- Cleans and normalizes legal document text
- Handles document length limitations (512 tokens max)

### 2. **Sentiment Analysis Pipeline**
- **Primary Model**: RoBERTa (Twitter-based sentiment analysis)
- **Legal Model**: FinBERT (Financial/Legal domain-specific analysis)
- **Fallback**: BERT Multilingual model for enhanced coverage

### 3. **Risk Assessment Algorithm**
- **High Risk**: Negative sentiment in both models with confidence > 80%
- **Medium Risk**: Negative sentiment in one model or moderate confidence (60-80%)
- **Low Risk**: Positive/neutral sentiment with acceptable confidence levels

### 4. **Visualization Engine**
- Interactive charts using Plotly
- Sentiment distribution pie charts
- Risk level bar charts
- Confidence score histograms

## 🛠️ Technical Details

### Models Used
- **cardiffnlp/twitter-roberta-base-sentiment-latest**: Primary sentiment analysis
- **ProsusAI/finbert**: Legal and financial domain analysis
- **nlptown/bert-base-multilingual-uncased-sentiment**: Fallback model

### Key Components
- `LegalSentimentAnalyzer`: Main analysis class
- `analyze_single_document()`: Individual document processing
- `analyze_multiple_documents()`: Batch processing functionality
- `create_visualizations()`: Interactive chart generation
- `assess_risk()`: Risk level calculation algorithm

## 📊 Output Examples

### Individual Analysis Results
- **Primary Sentiment**: Positive/Negative/Neutral classification
- **Confidence Score**: Percentage confidence in sentiment prediction
- **Legal Sentiment**: Domain-specific sentiment analysis
- **Legal Confidence**: Confidence in legal sentiment prediction
- **Risk Level**: High/Medium/Low risk assessment
- **Summary**: Actionable insights and recommendations

### Batch Analysis Results
- **Comprehensive Summary**: Total documents analyzed, sentiment distribution
- **Risk Assessment**: Breakdown of risk levels across all documents
- **Average Confidence**: Overall confidence metrics
- **Detailed Results Table**: Document-by-document analysis
- **Interactive Dashboard**: Visual analytics with multiple chart types

![Sample Output](https://via.placeholder.com/800x400/6f42c1/ffffff?text=Sample+Analysis+Output)
*Add your actual output screenshots here*

## 📈 Future Improvements

- [ ] Integration with document management systems
- [ ] Custom model training for specific legal domains
- [ ] Export functionality (PDF, CSV, Word)
- [ ] API endpoints for integration
- [ ] Multi-language support expansion
- [ ] Advanced risk scoring algorithms
- [ ] Cloud deployment options

## 👥 Contributing

We welcome contributions from the legal and AI communities:

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/legal-enhancement`)
3. Commit your changes (`git commit -m 'Add legal document classifier'`)
4. Push to the branch (`git push origin feature/legal-enhancement`)
5. Open a Pull Request

## 📞 Contact

Feel free to reach out if you have questions, suggestions, or would like to contribute:

- **GitHub**: [Open an issue](https://github.com/yourusername/legal-sentiment-analysis/issues)
- **Email**: aryankaminwar@gmail.com
- **LinkedIn**: [Your LinkedIn Profile](https://linkedin.com/in/yourprofile)

## 🔒 Privacy

The Legal Document Sentiment Analysis tool:
- Performs all analysis locally on your device
- Does not collect or transmit user data
- Does not share documents with any third parties
- Requires only necessary permissions to function properly

## 🙏 Acknowledgments

- **Hugging Face**: For providing the transformer models
- **Gradio Team**: For the excellent web interface framework
- **Legal Community**: For domain expertise and feedback
- **Open Source Contributors**: For continuous improvements
