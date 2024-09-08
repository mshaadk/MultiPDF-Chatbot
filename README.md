# LLM-Powered Multi-PDF Chatbot
A Streamlit application that allows users to interact with the content of multiple PDF files using Google's Gemini Model. This chatbot extracts text from PDF documents, processes it, and enables users to ask questions based on the content of the uploaded PDFs.

## Features
- **PDF Upload:** Users can upload multiple PDF files.
- **Text Extraction:** Extracts text from the uploaded PDFs.
- **Text Chunking:** Splits the extracted text into manageable chunks.
- **Vector Storage:** Stores text chunks in a vector store for efficient similarity searches.
- **Question Answering:** Uses a generative AI model to answer questions based on the content of the PDFs.

## Technologies Used
- **Streamlit:** For creating the web application.
- **PyPDF2:** For reading and extracting text from PDF files.
- **LangChain:** For text splitting, vector storage, and question answering.
- **FAISS:** For efficient similarity search.
- **Google's Gemini Model:** For embeddings and question answering.

## Setup Instructions
### Installation

#### 1. Clone the Repository

```bash
git clone https://github.com/mshaadk/MultiPDF-Chatbot.git
cd MultiPDF-Chatbot
```

#### 2. Create and Activate a Virtual Environment

```bash
python -m venv venv
source venv/bin/activate  # On Windows, use `venv\Scripts\activate`
```

#### 3. Install Required Packages

```bash
pip install -r requirements.txt
```

#### 4. Set Up Environment Variables

Create a `.env` file in the project root and add your Google API key:

```env
GOOGLE_API_KEY=your_google_api_key
```

#### 5. Run the Application

```bash
streamlit run app.py
```

## Usage
1. **Upload PDF Files:** Use the file uploader in the sidebar to upload your PDF documents.
2. **Process PDFs:** Click the "Submit & Process" button to extract and process the text from the PDFs.
3. **Ask Questions:** Enter your questions in the text input box and get answers based on the content of the uploaded PDFs.

## Contact
- Author: **Mohamed Shaad**
- LinkedIn: [mohamedshaad](https://www.linkedin.com/in/mohamedshaad/)
- GitHub: [mshaadk](https://github.com/mshaadk)

## License
This project is licensed under the MIT License. See the [LICENSE](LICENSE.txt) file for details.
