🚀 Multimodal RAG Application with FastAPI and Streamlit
This project implements a Multimodal Retrieval-Augmented Generation (RAG) System that processes document-based queries by leveraging multiple OCR methods, search techniques, and LLMs to provide accurate responses. The system is built using FastAPI for backend APIs and Streamlit for an intuitive user interface.

🎯 Key Features
📄 Document Upload & Selection:

Supports multiple file uploads with document-based query processing.

Users can selectively include/exclude files via a checkbox interface.

🧠 LLM Selection:

Integrates 5 LLMs: Qwen, Claude, GPT, Gemini, and Nvidia.

🔍 OCR Methods:

Supports 5 OCR options: Florence, Tesseract, GPT, Claude, and Google Vision.

Florence OCR integrated via a custom florence.py module.

🔎 Search Methods:

Implements 3 search techniques: BM25S, Semantic Qwen, and RRF Rank Fusion Hybrid Search.

🧩 Dynamic Context Processing:

Selectively processes document context based on user queries, optimizing response accuracy and latency.

💬 Dual API Architecture:

main API for core functionalities and chatapi for handling chat-based interactions.

🎛️ Streamlit Interface:

Two horizontal tabs:

Configuration Tab: Select LLM, search method, OCR method, and upload files.

Chat Tab: Engage in conversations with documents as the knowledge source.

Popover used for file and model selection to maintain a clean UI.

🛠️ Tech Stack
Backend: FastAPI

Frontend: Streamlit

Models: Azure Chat, Claude 3 Sonnet, Qwen, and others

OCR: Florence, Tesseract, GPT, Claude, Google Vision

Search Methods: BM25S, Semantic Qwen, RRF Rank Fusion

📚 How It Works
Upload Documents: Users upload multiple files via Streamlit. Selected files are considered for OCR and context extraction.

Configure Models & Methods: Choose desired LLM, OCR method, and search technique.

Ask Queries: User queries trigger document-based search and context processing.

Generate Response: Relevant content is passed to the chosen LLM to generate a contextualized answer.

