# Llama2_Medical_Chatbot_using_PineconeDB_and_Langchain

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