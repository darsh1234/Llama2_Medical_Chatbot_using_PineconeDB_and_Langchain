# Llama2_Medical_Chatbot_using_PineconeDB_and_Langchain

## Description

This project is a medical chatbot that combines the power of Llama2, a large language model trained on a vast corpus of text data including medical literature, with the efficiency of PineconeDB, a vector database used for storing and retrieving medical data. The chatbot leverages the Retrieval Augmented Generation (RAG) approach, where Llama2 generates responses based on both its pre-trained knowledge and relevant information retrieved from the PineconeDB index. Langchain, a framework for building applications with large language models, provides utilities for text generation, question answering, and data retrieval. The chatbot is designed to assist users with medical queries, providing accurate and relevant information by seamlessly integrating Llama2's language generation capabilities with the retrieved medical data from PineconeDB. Users can interact with the chatbot through a web interface, asking questions or seeking information on various medical topics. The RAG approach ensures that the chatbot's responses are not only fluent and contextually relevant but also factually grounded in the stored medical data.


## Installation

### 1. Clone the repository
```bash
git clone https://github.com/darsh1234/Llama2_Medical_Chatbot_using_PineconeDB_and_Langchain.git
```

### 2. create and activate environment
``` bash 
conda create -n medchatbot python=3.10 -y 
```

``` bash 
conda activate medchatbot 
```

### 3. install depenedencies
``` bash 
pip install -r requirements.txt
```

### 4. set envrionment variables
#### Create a .env file in the root directory and add your Pinecone credentials as follows:
```ini
PINECONE_API_KEY = ""
PINECONE_API_ENV = ""
```

### 5. Download the quantized LLama 2 Model:

TheBloke/Llama-2-7B-Chat-GGML

llama-2-7b-chat.ggmlv3.q4_0.bin

from the following link:
https://huggingface.co/TheBloke/Llama-2-7B-Chat-GGML/blob/main/llama-2-7b-chat.ggmlv3.q4_0.bin

Keep the model in model directory

### 6. Store your data in pinecone:

``` bash 
python store_index.py
```

### 7. Run the website and open local host:
``` bash 
python app.py
```
