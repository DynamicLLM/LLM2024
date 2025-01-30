**Install Ollama**

Windows: 

1. Head to Ollama’s download pageLinks to an external site. to download the Ollama installation file. Ollama binds 127.0.0.1 port 11434 by default. Change the bind address with the OLLAMA_HOST environment variable: setx OLLAMA_HOST 0.0.0.0:11434, before Ollama starts.  You can confirm the Ollama server status by hitting the local URL http://localhost:11434 or  http://yourIP:11434 

2. Open a windows terminal (command-prompt) and execute the following Ollama command:   ollama run llama3.1.  Now you can have interactive conversations with LLama3.1. 

3. See https://huggingface.co/docs/hub/en/ollama for run Hugg Face models with Ollama. For example: ollama run hf.co/bartowski/Llama-3.2-3B-Instruct-GGUF:latest. Use ollama list to see available models.  

4. You can call the llama3* in Python  https://github.com/DynamicLLM/LLM2024/blob/main/src/sample-ai-agent/Ollama_sample12_15.ipynb
 
Unix: 

install ollama 

module load ollama/0.1.38

export OLLAMA_HOST='10.139.120.41:11434'

ollama server 

curl http://10.139.121.74:11434

At server:  

Request a jupyter session with a GPU.

Open a terminal tab on jupyter lab.

Load the ollama-0.1.38 module.

Run ollama server.

Open a second terminal and download the llama3.1 model by running ollama pull llama3.1 .

Open a jupyter notebook and use the ollama-0.1.38 kernel.

