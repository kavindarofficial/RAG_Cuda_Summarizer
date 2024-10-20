# My CUDA RAG Project

## Requirements
To run my project, you will need the following:

- **Python 3.x**
- **Google Colab** (for easy setup and execution)
- **Ollama**
- **Mistral LLM model**

## Installation
To get started, I recommend cloning this repository or creating a new Colab notebook. Here’s how I set it up:

1. **Clone the repository or create a new Colab notebook.**

2. **Install the required Python packages**:
   I use the following command to install the necessary packages:
   ```bash
   !pip install -r requirements.txt
   ```
   The `requirements.txt` file should contain the following:
   ```
   pypdf
   langchain
   chromadb
   pytest
   boto3
   colab-xterm
   langchain_community
   langchain-chroma
   langchain-ollama
   ```

3. **Set up Ollama**:
   I perform the following steps to set up Ollama:

   a. Load the Colab terminal extension:
   ```bash
   %load_ext colabxterm
   ```

   b. Launch the terminal:
   ```bash
   %xterm
   ```

   c. In the terminal, I install Ollama using:
   ```bash
   curl https://ollama.ai/install.sh | sh
   ```

   d. Start the Ollama server:
   ```bash
   ollama serve
   ```

   e. Open a new terminal and pull the Mistral model(Run this after the execution of the previous step 'c'):
   ```bash
   ollama pull mistral
   ```

## Usage
Once the setup is complete, you can use the interactive notebook to query the model. Simply enter the questions, and the system provides responses based on the context of the document uploaded. This makes it easy to retrieve relevant information quickly!
Be patient while the response is generated and it will take a couple of minutes.

## Project Structure
The project is organized as follows:
```
cuda-rag-project/
│
├── cuda_docs/              # Directory for PDF documents
├── rag_cuda.ipynb          # Jupyter notebook for the project
└── requirements.txt         # Python packages required
```

## Customization
Feel free to customize the chunk size and overlap settings in the code to optimize performance based on your specific needs. I have made adjustments that can enhance processing speed and efficiency when working with large datasets.

## Notes
If you encounter any issues during setup or execution, please feel free to reach out. I appreciate any feedback or suggestions for improvements!

Thank you for checking out my project!
```
