# Code Assistant Application (CodeLlama-LLAMA2)


## Acknowledgement
I would like to extend my sincere thanks to  **[Krish Naik](https://github.com/krishnaik06)**  for his invaluable content and guidance, which helped me build this project. This project wouldn't have been possible without his educational resources.

<br>

## About the Project
This project leverages **[Ollama's](https://ollama.com/) [CodeLlama](https://ollama.com/library/codellama), [LangChain](https://www.langchain.com/)**, and **[Gradio](https://www.gradio.app/)** to build an interactive AI-powered coding assistant. The core functionality revolves around generating responses based on user prompts, with a persistent history to ensure context-aware replies.

### Key Components :

-   **Ollama's CodeLlama** : It provided the foundation for code generation, enabling AI-powered insights and suggestions.
-   **LangChain** : Used for enhancing prompt management and maintaining conversational memory, making interactions more coherent.
-   **Gradio** : A simple yet powerful interface for user interaction, allowing seamless prompt input and response display.

<br>

## How to Run the Project ?
(NOTE : This project was carried out on a [Macintosh](https://www.apple.com/mac/) machine)
### **1. Clone the Repository**
Clone the repository to your local machine :
```bash
git clone https://github.com/SoubhikSinha/Code-Assistant-Application-CodeLlama-LLAMA2.git

```

<br>

### **2. Create a Virtual Environment**
Navigate to the repository's root directory and create a Conda virtual environment :
```bash
conda create -p ./venv python=3.11 -y
```

<br>

### **3. Activate the Conda Environment**
Activate the newly created environment :
```bash
conda activate venv/
```

<br>

### **4. Install Required Libraries**
Install all the necessary dependencies :
```bash
pip install -r requirements.txt
```

<br>

### **5. Install Ollama**
Ollama is required to run the CodeLlama model. Follow the official installation guide for your operating system:
-   Install Ollama : https://ollama.com/download
<br>

After successful installation, verify the installation by running :
```bash
ollama --version
```

<br>

### **6. Run CodeLlama Model**
Once Ollama is installed, run the following command to execute CodeLlama :
```bash
ollama run CodeLlama
```

<br>

### **7. Create a Custom Model (CodeGuru)**
Generate a new custom model named "codeguru" using the `modelfile`:
```bash
ollama create codeguru -f modelfile
```

<br>

### **8. Run the CodeGuru Model**
Execute the following command to run the newly created `codeguru` model :
```bash
ollama run codeguru
```

<br>

### **9. Launch the Gradio Interface**
Finally, start the Python application to launch the Gradio-based interface :
```bash
python app.py
```
Once executed, the application will be available for interaction via a web-based interface.
