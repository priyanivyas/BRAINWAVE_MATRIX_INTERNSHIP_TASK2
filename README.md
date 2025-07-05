## Project: Twitter Sentiment Analysis


## Technical Skills
- **Languages:** Python, SQL
- **Data Analysis:** Pandas, NumPy, Matplotlib, Seaborn
- **Machine Learning:** Scikit-learn, Natural Language Processing
- **Tools:**  Google Colab

### Key Components

**Data Processing & Cleaning**
```python
def clean_text_for_eda(text):
    """
    Performs comprehensive text preprocessing:
    - Removes URLs, mentions, and hashtags
    - Converts to lowercase and normalizes whitespace
    """
    text = re.sub(r'http\S+|www\S+|https\S+', '', text, flags=re.MULTILINE)
    text = re.sub(r'@\w+', '', text)
    text = re.sub(r'#', '', text)
    text = text.lower()
    text = re.sub(r'\s+', ' ', text).strip()
    return text
```

**Statistical Analysis & Visualization**
- Sentiment distribution analysis across multiple entities
- Entity-based sentiment mapping with percentage calculations
- Text length distribution analysis
- Word frequency analysis with stopword filtering
- Professional visualizations using Seaborn and Matplotlib

**Data Quality Assurance**
- Automated missing value detection and handling
- Duplicate record identification and removal
- Data type validation and conversion
- Comprehensive error handling for file operations

### Technical Implementation
- **Data Loading:** Robust CSV processing with custom column mapping
- **Preprocessing:** Regex-based text cleaning and normalization
- **Analysis:** Multi-dimensional sentiment analysis across entities
- **Visualization:** Custom styling with seaborn-darkgrid theme
- **Error Handling:** Graceful fallback with dummy data generation


