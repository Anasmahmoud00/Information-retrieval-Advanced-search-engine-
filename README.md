# Hospital Search Engine

An advanced search engine specifically designed for hospital and medical information retrieval, utilizing BERT and PyTerrier for enhanced search capabilities.

## Features

- **Query Expansion**: Implements RM3 query expansion to improve search relevance
- **BERT-based Reranking**: Uses BERT model for intelligent result reranking
- **Web Interface**: Clean and responsive Flask-based web interface
- **Real-time Search**: Fast and efficient search with performance metrics
- **Document Viewer**: Dedicated view for detailed document content

## Technologies Used

- **Backend Framework**: Flask
- **Search Framework**: PyTerrier
- **Machine Learning**: BERT (bert-base-uncased)
- **Natural Language Processing**: NLTK
- **Frontend**: HTML/CSS with responsive design
- **External Services**: ngrok for tunneling

## Prerequisites

Before running this project, make sure you have the following installed:

- Python 3.7+
- pip package manager
- Virtual environment (recommended)

## Installation

1. Clone the repository:
```bash
git clone [your-repository-url]
cd hospital-search-engine
```

2. Install required packages:
```bash
pip install -r requirements.txt
```

3. Download required NLTK data:
```python
import nltk
nltk.download('stopwords')
nltk.download('punkt')
```

4. Set up ngrok:
- Sign up for ngrok account
- Get your authentication token
- Replace the token in the code with your own token

## Usage

1. Start the application:
```bash
python app.py
```

2. Access the application:
- The application will start on a local port
- ngrok will create a public URL that you can use to access the application
- The URL will be displayed in the console when you start the application

3. Using the search interface:
- Enter your search query in the search box
- Click "Search" or press Enter
- View results with relevance scores
- Click on individual results to view full document content

## Search Features

### Query Processing
- Text preprocessing
- Stopword removal
- Porter stemming
- Query expansion using RM3

### Ranking System
1. Initial ranking using TF-IDF
2. BERT-based reranking for improved relevance
3. Combined score calculation for final ranking

## Performance

The search engine provides:
- Number of results found
- Search execution time
- BERT-based relevance scores

## File Structure

```
hospital-search-engine/
├── app.py              # Main application file
├── index/             # PyTerrier index directory
├── static/            # Static files (CSS, images)
├── templates/         # HTML templates
└── requirements.txt   # Project dependencies
```

## Contributing

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request



