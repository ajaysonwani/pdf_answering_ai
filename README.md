## Here is the streamlit deployed app link- https://pdfansweringai-7wmhdc9uzgenccskbb4auy.streamlit.app/
Please Follow instruction.txt for make model to work.
# Chat with Multiple PDFs

This project involves a Streamlit-based application enabling users to interact with multiple PDF documents through a chat interface. It employs FAISS for efficient document retrieval and utilizes a T5 model to generate responses. The PDF documents are processed, with their text divided into manageable chunks, vectorized, and stored in a FAISS index. Users can then pose questions, and the system retrieves relevant document sections to generate accurate and contextually relevant responses.


## Features

- Upload and process multiple PDF files.
- Extract text from PDFs and divide it into chunks.
- Vectorize the text chunks using SentenceTransformers.
- Store and retrieve text chunks using FAISS.
- Generate responses using a local T5 model.
- Provide an interactive chat interface with document preview.

## Prerequisites

- Python 3.7 or higher

 Required Python packages (see `requirements.txt`)

## Installation

1. Clone the repository:
    ```bash
    git clone https://github.com/ajaysonwani/pdf_answering_ai.git
    cd yourrepository
    ```

2. Create a virtual environment and activate it:
    ```bash
    python -m venv venv
    source venv/bin/activate  # On Windows use `venv\Scripts\activate`
    ```

3. Install the required packages:
    ```bash
    pip install -r requirements.txt
    ```

4. Download the LaMini-T5-738M model and place it in your project directory:
    - Place the model files in a directory, e.g., `models/LaMini-T5-738M`

## Usage

1. Run the Streamlit app:
    ```bash
    streamlit run app.py
    ```

2. Open your web browser


4. Upload your PDF files using the sidebar, click "Process", and wait for processing to complete.


6. Ask questions about the uploaded documents in the main chat interface.
   Note: Please Download "MBZUAI/LaMini-T5-738M" model from hugging face at your folder location using code from trial.ipynb

## File Structure

- `app.py`: Main application code.
- `Templates.py`: HTML and CSS templates for the chat interface.
- `requirements.txt`: List of required Python packages.

## Code Explanation

### app.py

- **FAISSRetriever Class**: Handles the retrieval of relevant documents from the FAISS index.
- **get_pdf_text**: Extracts text from uploaded PDF files.
- **get_text_chunks**: Splits extracted text into manageable chunks.
- **get_vectorstore**: Vectorizes text chunks and stores them in a FAISS index.
- **get_conversation_model**: Loads the local T5 model for generating responses.
- **generate_response**: Generates a response to the user's query using the T5 model.
- **main**: Streamlit app main function that handles file uploads, processing, and chat interface.

### Templates.py

- **CSS and HTML Templates**: Contains the styles and structure for the chat interface, including user and bot message templates and the PDF preview window.
- **render_pdf**: Function to render PDF files in an iframe for preview.


## Acknowledgements

- [Streamlit](https://streamlit.io/)
- [SentenceTransformers](https://www.sbert.net/)
- [FAISS](https://faiss.ai/)
- [Hugging Face](https://huggingface.co/)


https://github.com/ajaysonwani/pdf_answering_ai


https://github.com/ajaysonwani/pdf_answering_ai/assets/109919149/aa2c96b1-9019-4fb9-bf5d-f9dfbf8175bc


  

