# TOPSIS for Text Summarization

## Overview
This project utilizes the TOPSIS (Technique for Order of Preference by Similarity to Ideal Solution) method for text summarization. It aims to provide a systematic approach for selecting the best text summarization model based on multiple criteria.

### **TOPSIS**




TOPSIS (Technique for Order of Preference by Similarity to Ideal Solution) is a decision-making method used to choose the best alternative from a set of options. It involves:

- **Normalization:** Scaling criteria to a common range for fair comparison.


- **Weighting:** Assigning weights to criteria based on their importance.


- **Positive and Negative Ideal Solutions:** Determining the best and worst possible values for each criterion.


- **Distance Calculation:** Measuring the distance of each alternative to both ideal solutions.


- **Ranking:** Assigning a preference ranking based on the calculated distances.

### **TEXT SUMMARIZATION**


Text summarization is the process of condensing a piece of text, preserving its key information, while reducing its length. There are two main types of text summarization:

- **Extractive Summarization:** Selects and extracts sentences or phrases directly from the original text to form a summary.
Uses algorithms to identify and rank sentences based on their importance.


- **Abstractive Summarization:** Generates a summary by paraphrasing and rephrasing the content in a new way.
Involves understanding the meaning of the text and generating novel sentences.


Text summarization is employed in various applications, such as:

- News Articles: Creating concise summaries of news articles for quick information retrieval.
- Legal Documents: Condensing lengthy legal documents to extract key points and arguments.
- Research Papers: Providing a brief overview of complex research findings.
- Search Engine Snippets: Generating concise summaries for search engine results.
- Content Aggregation: Summarizing and presenting content from multiple sources in a condensed form.

## Features

- Apply the TOPSIS method to rank text summarization models.
- Compare models based on criteria such as Rouge Scores, Length of Summary, and Training Time.
- Visualize model rankings using bar charts.

## Getting Started

### Prerequisites

- Python 3.x
- pandas
- numpy
- matplotlib
- seaborn

### How to run the project

 Clone the repository:
1. **Clone the Repository:**
   ```bash
   git clone https://github.com/MannatPruthi/Topsis-for-pre-trained-models.git

## Results and Analysis:

### **1. Ranked Table**

| Model      | Rouge Scores | Length of Summary | Training Time | TOPSIS Score | Rank |
|------------|--------------|-------------------|---------------|--------------|------|
| BERTSumExt | 0.75         | 130               | 9             | 0.723580353  | 2    |
| GPT-3      | 0.82         | 150               | 12            | 0.276419647  | 5    |
| T5         | 0.78         | 140               | 10            | 0.578940666  | 3    |
| BART       | 0.80         | 145               | 8             | 0.790404602  | 1    |
| Pegasus    | 0.79         | 138               | 13            | 0.202345744  | 6    |
| UniLM      | 0.75         | 130               | 12            | 0.321878943  | 4    |

### **2. Bar Graph**

The bar chart visually represents the performance metrics of each model, providing an easy-to-understand comparison. Rouge scores, length of the summary, training time, and normalized ranks are included for comprehensive evaluation.

![barchart](https://github.com/MannatPruthi/Topsis-for-pre-trained-models/assets/91721574/8d87abaa-8828-44c5-82be-bd87119b7bd8)

![bargraph](https://github.com/MannatPruthi/Topsis-for-pre-trained-models/assets/91721574/a68dac89-b2f4-4212-98b0-b11a36bcda96)


### **3. Analysis**

**Model Performance:**
- BART emerges as the top-performing model with the highest Rouge score, leading to the first rank.
- T5 closely follows, securing the third rank, demonstrating competitive Rouge scores and a commendable TOPSIS score.
- BERTSumExt and UniLM perform similarly in Rouge scores, ranking second and fourth, respectively.
- GPT-3, despite having a high Rouge score, ranks lower in TOPSIS due to its relatively low TOPSIS score.
- Pegasus, while having a decent Rouge score, ranks the lowest in both TOPSIS and overall rank.

**Efficiency Consideration:**
- BERTSumExt stands out as the most resource-efficient model, having the lowest training time.
- BART, despite achieving the top Rouge score, is also efficient with a moderate training time.
- T5 and UniLM offer a balance between Rouge scores and efficiency, with moderate training times.
- GPT-3 and Pegasus have longer training times, impacting their efficiency.

**Next Steps:**
- Dive deeper into the provided CSV files to gain a comprehensive understanding of each model's performance across various criteria.
- Consider adjusting the evaluation metrics based on your specific use case and requirements.
- Explore the possibility of adding new models to the comparison for a more comprehensive analysis.
- Utilize this project as a foundation for ongoing research and development in the field of text summarization.
