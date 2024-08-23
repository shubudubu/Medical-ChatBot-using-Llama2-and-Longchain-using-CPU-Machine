Healthcare ChatBot - Powered by LLaMA 2 and LangChain
Description:
This project is a Healthcare ChatBot designed to assist users by answering their queries related to healthcare and mental well-being. It leverages state-of-the-art language models and retrieval-based natural language processing techniques, making it a powerful tool for personalized healthcare advice and information.

Key Features:

Conversational AI: Utilizes the LLaMA 2 language model to generate human-like responses, enabling users to have meaningful and informative conversations about their health.
Conversational Retrieval Chain: Powered by LangChain’s ConversationalRetrievalChain, the bot can retrieve and provide relevant information from a collection of healthcare documents stored in PDF format. This ensures the chatbot can reference specific and accurate details when responding to user inquiries.
PDF Document Integration: The chatbot is integrated with a PDF loader that ingests healthcare-related documents, breaking them into manageable chunks for efficient information retrieval and response generation.
Custom Embeddings: Uses HuggingFace’s sentence-transformers/all-MiniLM-L6-v2 model to create embeddings for the document chunks, ensuring precise matching and retrieval of relevant information.
FAISS Vector Store: Implements FAISS (Facebook AI Similarity Search) to store and retrieve vectorized documents, enabling fast and accurate searches within the provided healthcare documents.
Session Memory: Incorporates a conversation buffer memory to maintain context across user interactions, allowing the chatbot to reference previous conversations for a coherent and continuous experience.
Streamlit Integration: Built using Streamlit, providing a user-friendly web interface where users can interact with the chatbot seamlessly. The chat interface is intuitive, displaying the conversation history with user inputs and bot responses.
How It Works:

Loading Documents: The bot loads healthcare-related PDF documents from the specified directory, which are then split into smaller text chunks for easier processing.
Embeddings and Vector Store: Each text chunk is embedded using a sentence transformer model, and these embeddings are stored in a FAISS vector store, allowing the bot to quickly retrieve relevant information.
LLaMA 2 Language Model: The chatbot uses the LLaMA 2 model to generate responses based on user queries and the retrieved document chunks, providing accurate and context-aware answers.
Chat Interface: Users can interact with the chatbot through a simple and elegant Streamlit interface, where they can ask health-related questions and receive responses in real time.
Example Commands:

Ask questions like "What are the symptoms of anxiety?" or "How can I improve my mental health?" to get instant, accurate answers based on the healthcare documents loaded into the bot.
Technology Stack:

Language Model: LLaMA 2 (7B) via CTransformers
Document Processing: PyPDFLoader and RecursiveCharacterTextSplitter
Embeddings: HuggingFace Sentence Transformers
Vector Store: FAISS
Memory: ConversationBufferMemory
Web Interface: Streamlit and Streamlit Chat
Usage:

Run the Application: Deploy the chatbot on a local server or in a cloud environment using Streamlit.
Interact: Start a conversation with the bot, asking health-related questions. The bot retrieves information from the documents and provides accurate, context-aware responses.
Review Chat History: The bot keeps track of previous interactions to maintain the conversation flow, making it easy for users to continue where they left off.
This chatbot is a cutting-edge example of how advanced language models and retrieval systems can be applied in the healthcare domain, offering users a reliable source of information while engaging them in meaningful dialogue.

![healthcareBotImage](https://github.com/InsightEdge01/LLama2HealthCareChatBot/assets/131486782/0f610cc4-8fda-456e-b4ce-4a871fe93936)
