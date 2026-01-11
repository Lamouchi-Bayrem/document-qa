📄 Document‑QA

A simple Document Question Answering web application built with Streamlit that allows users to upload documents and interactively ask questions about their content using OpenAI’s GPT‑3.5 (or compatible models).

🚀 Features

✅ Upload PDF or text documents and extract content
✅ Ask natural language questions about the document
✅ Get answers powered by GPT embedding + reasoning
✅ Interactive UI via Streamlit
✅ Fast local prototyping for document search and QA
✅ Easy to extend and adapt for RAG, vector DB, or custom LLMs

📦 Tech Stack

Frontend / UI: Streamlit

Backend: Python

Language Model: OpenAI GPT‑3.5 or similar

Document Parsing: Python libraries (PDF/Text)

Vector Search (optional): FAISS / other retrievers

Deployment: Local or cloud hosting

📁 Project Structure
document-qa/
├── .devcontainer/             # Dev container config (optional)
├── .github/                   # GitHub workflows (CI/CD)
├── requirements.txt           # Python dependencies
├── streamlit_app.py           # Main app entry point
├── README.md                 # Project documentation
├── LICENSE                   # Apache‑2.0 License
├── uploads/                  # (Optional) folder to store uploaded docs

🛠️ Installation

Clone the Repository

git clone https://github.com/Lamouchi-Bayrem/document-qa.git
cd document-qa


Create & Activate Virtual Environment

python3 -m venv .venv
source .venv/bin/activate   # macOS / Linux
.venv\Scripts\activate      # Windows


Install Dependencies

pip install -r requirements.txt

▶️ Running the App

Start the Streamlit UI:

streamlit run streamlit_app.py


Once launched, a browser window will open with the document upload interface and chat input.

📌 Usage Guide

Upload your document (PDF, text) using the Streamlit UI.

Wait for the content to be parsed and loaded.

Enter your question in the chat input field.

View the generated answer from the LLM.

Improve responses by providing high‑quality documents or extending retrieval.

🧠 How It Works (Concept)

Document Upload – User uploads a PDF/text file.

Text Extraction – Transform the document into searchable text.

Embedding / Retrieval – Convert document content into embeddings for semantic search (optional).

LLM Query – Ask natural language questions; the model responds using the document context.

⚙️ Customization & Extensions

Add vector database support (e.g., FAISS) for efficient retrieval.

Extend to support more formats (DOCX, PPTX, images with OCR).

Use alternative NLP models or fine‑tuned embeddings.

Deploy via Docker, Heroku, or Cloud Services.

🤝 Contributing

Contributions are welcome! To contribute, please:

Fork this repository

Create a new branch (feat/your‑feature)

Commit your changes

Push your branch

Open a Pull Request

Please ensure PRs include clear descriptions and follow the repository style.

🧪 License

This project is open source and licensed under the Apache‑2.0 License. See the LICENSE file for details.

❤️ Acknowledgements

Thanks to the open‑source community and the original Streamlit Document‑QA template for the base structure.
