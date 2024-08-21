# **Development of Data Scraping and Collection Mechanisms for AI and Cybersecurity Research Articles**

## **Table of Contents**
- [Project Overview](#project-overview)
- [Features](#features)
- [Technologies Used](#technologies-used)
- [Installation](#installation)
- [Usage](#usage)
- [Project Structure](#project-structure)
- [Results](#results)
- [Challenges and Solutions](#challenges-and-solutions)
- [Future Work](#future-work)
- [Contributors](#contributors)
- [License](#license)

## **Project Overview**
This project focuses on automating the collection, categorization, and dissemination of research articles related to Artificial Intelligence (AI) and cybersecurity. By leveraging data scraping, machine learning, and topic modeling techniques, the system provides personalized article recommendations and aids in keeping users informed about the latest research trends.

## **Features**
- **Data Collection:**
  - Automated scraping of metadata from research platforms like arXiv, IEEE Xplore, and Springer.
  - Storage of collected data in an organized and structured format using SQLite.
  
- **Data Preprocessing:**
  - Text cleaning, stop word removal, stemming, and lemmatization.
  - Vectorization using TF-IDF for machine learning model training.

- **Machine Learning:**
  - Implementation of Naive Bayes and Support Vector Machines (SVM) for article categorization.
  - Initial integration of Deep Learning models (e.g., BERT) to improve categorization accuracy.

- **Topic Modeling:**
  - Utilization of Latent Dirichlet Allocation (LDA) for discovering key topics in the dataset.

## **Technologies Used**
- **Programming Languages:** Python
- **Libraries and Tools:** 
  - Data Scraping: BeautifulSoup, Scrapy, Selenium
  - Data Analysis: pandas, numpy
  - Machine Learning: scikit-learn, TensorFlow, PyTorch
  - Topic Modeling: gensim (for LDA)
- **APIs:** arXiv API, IEEE Xplore API, Springer API
- **Database:** SQLite
- **Development Environment:** PyCharm IDE, Jupyter Notebook

## **Installation**
To set up the project locally, follow these steps:

1. Clone the repository:
   ```bash
   git clone https://github.com/Rama0surya/Data-Scraping-and-Collection-Mechanisms.git
   cd Data-Scraping-and-Collection-Mechanisms
   ```

2. Create a virtual environment:
   ```bash
   python3 -m venv env
   source env/bin/activate  # On Windows use `env\Scripts\activate`
   ```

3. Install the required dependencies:
   ```bash
   pip install -r requirements.txt
   ```

4. Set up your API keys for arXiv, IEEE Xplore, and Springer in the environment variables or in a configuration file.

## **Usage**
1. **Data Collection:**
   - Run the data scraping scripts to collect metadata from arXiv, IEEE Xplore, and Springer.
   - Store the collected data in an SQLite database.

2. **Data Preprocessing:**
   - Clean the text data using the provided preprocessing script.
   - Vectorize the text data using TF-IDF.

3. **Machine Learning:**
   - Train the Naive Bayes and SVM models on the preprocessed data.
   - Evaluate the models' performance using accuracy metrics.

4. **Topic Modeling:**
   - Apply LDA to identify key topics within the dataset.

## **Project Structure**
```plaintext
├── data/
│   ├── raw/                 # Raw data collected from sources
│   ├── processed/           # Preprocessed and cleaned data
├── models/                  # Machine learning models and checkpoints
├── notebooks/               # Jupyter Notebooks for exploratory analysis
├── scripts/                 # Python scripts for data collection and processing
├── README.md                # Project README file
├── requirements.txt         # Python dependencies
└── LICENSE                  # License for the project
```

## **Results**
- **Data Collection:** Successfully gathered and stored metadata from major research platforms.
- **Preprocessing:** Achieved efficient text cleaning and vectorization.
- **Machine Learning:** 
  - Naive Bayes: 75% accuracy in article categorization.
  - SVM: 82% accuracy, showing improved performance.
- **Topic Modeling:** LDA successfully identified 10 coherent topics relevant to AI and cybersecurity.

## **Challenges and Solutions**
- **Rate Limits & Compliance:** Implemented API usage and delays to respect rate limits.
- **Library Integration:** Managed dependencies and setup using virtual environments.
- **Large Text Data Processing:** Leveraged pandas and efficient pipelines for preprocessing.

## **Future Work**
- Integrate more deep learning models to enhance categorization accuracy.
- Expand the dataset to include additional sources and topics.
- Improve the user interface for better accessibility and usability.

