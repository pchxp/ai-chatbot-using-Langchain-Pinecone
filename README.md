# Chatbot Answering from Your Own Knowledge Base: Langchain, ChatGPT, Pinecone, and Streamlit
![스크린샷 2024-03-13 145237](https://github.com/pchxp/ai-chatbot-using-Langchain-Pinecone/assets/31230133/7d0461a7-4f19-4c98-98b4-35a3971b8fac)
## Deployment

#### 1. Clone Repository 

```bash
  git clone https://github.com/pchxp/ai-chatbot-using-Langchain-Pinecone.git
```
```bash
  cd ai-chatbot-using-Langchain-Pinecone
```
#### 2. Create Virtual Environment
```bash
  python -m venv env
```
 - For Windows:
```bash
  .\env\Scripts\activate
```
 - For macOS/Linux:
```bash
  source env/bin/activate
```

#### 3. To install require packages 

```bash
  pip install -r requirements.txt
```
#### 4. Replace your own document in **data** folder

#### 5. Replace your own OpenAI, Pinecone API Key and Pinecone environment in indexing.py, main.py & utils.py
 - [OpenAI API Key](https://platform.openai.com)
 - [Pinecone](app.pinecone.io)

#### 6. When you are creating the pinecone index make sure,
   - **index_name = "langchain-chatbot"**
   - **Dimensions of the index is 384**

#### 7. Indexing to vectorDB(pinecone)
```bash
  python indexing.py
```
 
#### 8. Run the web app
```bash
  streamlit run main.py
```
