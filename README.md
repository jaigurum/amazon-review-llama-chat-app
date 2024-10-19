# Amazon Reviews Llama Model Chat Application

This repository contains a Streamlit-based application that leverages Llama language models to answer questions based on Amazon product reviews. The purpose of this project is to create an interactive platform where users can ask questions about Amazon products, and the Llama model will provide answers based on relevant customer feedback.

## Project Structure

```
├── notebooks/
│   ├── model_analysis.ipynb  # Notebook for evaluating model performance
│   └── data_preparation.ipynb  # Notebook for data cleaning and feature engineering
├── src/
│   ├── data_utils.py  # Utilities for data preprocessing
│   └── model_utils.py  # Utilities for model interaction and configuration
├── app.py  # Streamlit application file for interacting with the Llama model
├── README.md  # Project overview and instructions
```

## Features
- **Interactive Q&A**: Users can interact with the Llama model to ask questions about Amazon products.
- **Amazon Review Data**: Uses the Amazon Reviews 2023 dataset to provide answers based on real customer feedback.
- **Enhanced Contextual Responses**: The model is provided with contextual prompts and example Q&A to improve the relevance of its responses.
- **Sample Questions**: Users are provided with clickable sample questions to help initiate interaction.

## Setup Instructions

### Prerequisites
- Python 3.x
- Install the required dependencies:
  ```bash
  pip install -r requirements.txt
  ```
- Install the datasets library from Hugging Face:
  ```bash
  pip install datasets
  ```

### Pull the Llama Models
To use the Llama models in the application, pull the required models:
```bash
ollama pull llama3.1:8b
ollama pull llama3.2:1b
```

### Running the Application

To start the Streamlit application, run:
```bash
streamlit run app.py
```
This will launch the app in your browser, allowing you to ask questions about Amazon product reviews.

## Sample Questions
In the application, you can try asking questions like:
- **What do customers think about [product name]?**
- **Are there any common complaints about [product category]?**
- **How do people describe the durability of [product name]?**
- **What features are customers happy about in [product]?**

The questions are clickable in the sidebar, making it easier for users to get started quickly.

## Implementation Details

### Enhancements to Ensure Relevant Responses
- **Contextual Prompting**: The prompt is enhanced with additional context to clarify the task for the model, such as specifying it as an "Amazon review expert".
- **Few-Shot Prompting**: The model is provided with example questions and answers to guide it towards generating relevant responses.
- **Response Validation**: A validation mechanism is included to check if the response is relevant to the given question, ensuring higher quality and contextual accuracy.

## Data Preparation
The data preparation involves loading and cleaning the **Amazon Reviews 2023** dataset using the `datasets` library from Hugging Face.

- **Load Data**: The dataset is loaded and converted into a DataFrame for easier processing.
- **Data Cleaning**: Handles missing values and removes empty entries from the review data.
- **Feature Engineering**: Adds features such as `review_length` and `word_count` to enrich the dataset.
- **Save Processed Data**: The cleaned and processed data is saved to `processed_amazon_reviews_2023.csv` for further analysis and model training.

## Model Analysis
The `model_analysis.ipynb` notebook allows users to evaluate and benchmark the Llama models using the Amazon Reviews dataset. This includes:
- Loading the trained models.
- Running evaluations to understand model accuracy and efficiency.
- Analyzing response times and quality based on real customer questions.

## Contributing
Feel free to contribute by submitting issues or pull requests for additional features or enhancements.

## License
This project is licensed under the MIT License.
