# Streamlit Llama Chat Application

This project is an interactive chat application built using **Streamlit** that interacts with the **Llama language model** via **Ollama**. It demonstrates various data science skills, including deploying machine learning models, creating a web-based interface, and modularizing Python code to improve maintainability.

## Project Overview

The Streamlit Llama Chat App showcases the power of natural language processing through an interactive web interface. This project demonstrates the end-to-end process of developing a conversational AI, from integrating a model with a user-facing application to deploying it in a usable environment. It is designed as a portfolio project to showcase your data science skills for recruitment purposes.

## Features

- **Interactive Chat Interface**: Users can input text, and the app provides responses using the Llama language model.
- **Streamlit Web Interface**: Built using Streamlit to allow easy interaction with the language model.
- **Logging and Debugging**: Integrated logging to trace response generation and streamline debugging.
- **Modular Structure**: Separated application logic, data processing, and model interaction into different files for better maintainability.

## Directory Structure

```
streamlit-llama-chat-app/
├── llama-streamlit.py    # Main Streamlit application script
├── requirements.txt      # List of Python dependencies
├── README.md             # Project description, features, and usage instructions
├── Modelfile             # Model configuration for Ollama
├── notebooks/            # Jupyter notebooks for data exploration and analysis
│   ├── model_analysis.ipynb
│   └── data_preparation.ipynb
├── src/                  # Helper scripts for data and model utilities
│   ├── data_utils.py
│   └── model_utils.py
├── images/               # Images for README or documentation
├── .gitignore            # Files to ignore in Git
└── .github/workflows/    # CI/CD workflow for GitHub Actions
    └── streamlit.yml
```

## Setup Instructions

To set up and run the project locally, follow the steps below:

### Prerequisites

- **Python 3.x**: Ensure you have Python 3.x installed.
- **Git**: To clone the repository.

### Installation

1. **Clone the Repository**:
   ```bash
   git clone https://github.com/jaigurum/streamlit-llama-chat-app.git
   cd streamlit-llama-chat-app
   ```

2. **Install Dependencies**:
   Install the required Python libraries using:
   ```bash
   pip install -r requirements.txt
   ```

3. **Pull the Llama Model**:
   Use Ollama to pull the required Llama model:
   ```bash
   ollama pull llama3.1:8b
   ```

### Running the Application

To start the Streamlit application, run:
```bash
streamlit run llama-streamlit.py
```

This command will launch a local server. Navigate to the provided URL (usually `http://localhost:8501`) in your web browser to interact with the chat application.

## Example Usage

- Enter any question or statement in the chat input field.
- The Llama model will generate a response that will be displayed in the chat interface.

## Technologies Used

- **Streamlit**: Used for building an interactive web interface.
- **Python**: Main programming language.
- **Ollama**: For interacting with the Llama language model.
- **Jupyter Notebooks**: For data analysis and model experiments.
- **GitHub Actions**: For CI/CD integration to ensure code reliability.

## Project Highlights

- **Data Preparation and Exploration**: Jupyter notebooks (`notebooks/`) demonstrate your approach to data analysis, feature extraction, and model evaluation.
- **Modular Codebase**: The use of separate utility scripts (`src/`) for data and model operations showcases good software engineering practices.
- **Logging and Debugging**: Integrated logging into the app to assist in debugging and understanding user interactions.

## Future Improvements

- **Add Model Fine-Tuning**: Extend functionality to allow fine-tuning of the language model on custom datasets.
- **Deploy on the Cloud**: Deploy the application using a cloud service (e.g., AWS, GCP) to make it accessible publicly.
- **Implement User Authentication**: Allow users to sign in before accessing the app, improving usability for real-world deployment.

## Contributing

If you'd like to contribute to the project, feel free to fork the repository and submit a pull request. Contributions are welcome, especially on features like improving model performance and adding new user interface components.

## License

This project is open source and available under the [MIT License](LICENSE).

## Contact

If you have any questions or feedback, feel free to reach out!

- **Email**: [mjguru@gmail.com](mailto\:mjguru@gmail.com)
- **GitHub**: [jaigurum](https://github.com/jaigurum)

---

Thank you for checking out this project! If you found it useful or interesting, feel free to star the repository on GitHub.

