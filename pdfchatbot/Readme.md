# **PDF Chatbot**

## **Objective**

PDFChatbot is designed to answer 10th-grade Maths and Science questions using a ChatReactAgent with RAG pipeline implemented inside a notebook.

----

## **Implementation**

# **Method 1: Hugging Face Endpoint**

 • Uses Hugging Face Inference Endpoint with API token access.

 • Results are fetched directly from the hosted model.

 • Limitations: Free account has restrictions such as limited query checking, slower response, and capped usage.

 • Used **deepseek-ai/DeepSeek-R1-0528**
 
# **Method 2: Hugging Face Pipeline**

 • Runs locally with the Hugging Face pipeline API.

 • Uses a created access token for model loading.

 • Limitations: Token creation quota, no GPU on free tier, and large models cannot be easily used.

 • Used **HuggingFaceH4/zephyr-7b-beta**
   
   Both methods are wrapped with ChatHuggingFace so the agent can behave like a chat model and utilize its full potential.

   (Specific models used in Endpoint and Pipeline will be listed separately.)

---- 

## **Future Plans**

 • Extend to multi-subject QA.

 • Add proper deployment (Flask/FastAPI).

 • Enable large model support with GPU backend.

----- 

## **Tech Stack**

• LangChain

• FAISS (for vector search)

• Hugging Face Transformers

• Python

## **How to Run**

**1. Clone the repository**  
   
    git clone https://github.com/Gurushankar2025/langchain-rag-projects.git
    cd langchain-rag-projects/pdfchatbot

**2. Install dependencies**

    pip install -r requirements.txt
   
**3. Run the notebook**

    jupyter notebook PDF_Chatbot.ipynb
