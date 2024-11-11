
---

# T5 Chatbot for Customer Support

This project implements a customer support chatbot using a fine-tuned T5 model. The project includes the code for fine-tuning the T5 model and a web interface to deploy the chatbot. The model was trained on Kaggle with 2 GPUs and is publicly uploaded on Hugging Face. The web interface uses Hugging Face's API to send requests from HTML and receive responses from the model.

You can access the model on Hugging Face here: [T5 Chatbot Customer Support](https://huggingface.co/sunbv56/T5_Chatbot_CustomerSupport)

## Project Description

The project consists of two main parts:

1. **Fine-tuning the T5 Model**: The file `t5-chatbot-bitext-gen-ai-chatbot-customer-support.ipynb` contains the code for fine-tuning the T5 model. The model is trained to answer common customer support questions in a natural and accurate way. The model was trained on Kaggle with 2 GPUs.

2. **Web Interface Deployment**: The file `index.html` provides a simple user interface for the chatbot, allowing users to interact with the chatbot via a web interface. This web interface uses Hugging Face's API to send requests from HTML and receive responses from the trained model.

## Project Structure

- **t5-chatbot-bitext-gen-ai-chatbot-customer-support.ipynb**:
  - Data preprocessing for training.
  - Fine-tuning the T5 model on the customer support dataset.
  - Saving the fine-tuned model for use in the chatbot.

- **index.html**:
  - A simple user interface to interact with the chatbot via the web using Hugging Face’s API.

## Setting Up the Environment

1. **Clone the repository**:
   ```bash
   git clone https://github.com/sunbv56/T5-Chatbot-CustomerSupport.git
   cd T5-Chatbot-CustomerSupport
   ```

2. **Install the required libraries**:
   After setting up a virtual environment, install the necessary libraries using the following command:

   ```bash
   pip install -r requirements.txt
   ```

## Training the Model

1. **Open the `t5-chatbot-bitext-gen-ai-chatbot-customer-support.ipynb` file**:
   - Use Jupyter Notebook or Google Colab to open and run the notebook.
   - The notebook guides you through the process of fine-tuning the T5 model with the customer support dataset.
   - The model was trained on Kaggle with 2 GPUs and the results were uploaded to Hugging Face for public use.

2. **Run the entire notebook** to train the model:
   - From data preprocessing to fine-tuning the model.
   - After training, the model will be saved and uploaded to Hugging Face.

## Deploying the Web Interface

1. **Run the Web Interface**:
   - After fine-tuning the model, you can use the `index.html` file to deploy the chatbot web interface.
   - The web interface uses Hugging Face’s API to send requests and receive responses from the fine-tuned model.

2. **Sending requests from HTML**:
   - The web interface sends requests to the Hugging Face API to interact with the model and get responses.

## Libraries Used

- **evaluate**: For evaluating model performance.
- **sentence_transformers**: Used for sentence embedding and similarity calculations.
- **faiss-cpu**: Used for similarity search in vector space.
- **rouge_score**: For evaluating the quality of generated responses.
- **bert-score**: For scoring the generated text against reference text.
- **transformers**: The main library for working with the T5 model.
- **torch**: Deep learning framework used for model training and inference.
- **matplotlib, seaborn**: For visualizing results during analysis and evaluation.

## Contributing

Contributions are welcome! If you find any issues, have suggestions for improvements, or want to add new features, please create an issue or submit a pull request.

---
