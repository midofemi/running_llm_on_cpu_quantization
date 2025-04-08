# Running a Quantized LLaMA model utilizing CPU
This project is a PDF-based Question Answering chatbot powered by a quantized version of LLaMA 2, efficient vector retrieval using FAISS, and a simple Flask web interface. Users can interact with their documents by asking questions, and the system will retrieve relevant content and generate accurate answers using local models—no internet or API key required!

#### How to Run?

### Step 1-: Clone the Repository
```
git clone https://github.com/midofemi/running_llm_on_cpu_quantization.git
```

### Steps 2-: Create a Virtual Environment
```
conda create -n cpullama python=3.8 -y
```

### Step 3-: Activate Conda environment
```
conda activate cpullama
```

### Step 4-: Install requirements
```
pip install -r requirements.txt
```

### Step 5-: Download Quantized LLaMA 2 Model and place it in the model folder
```
llama-2-7b-chat.ggmlv3.q4_0.bin

https://huggingface.co/TheBloke/Llama-2-7B-Chat-GGML/tree/main
```

### Step 6-: Start the Application
```
python app.py
```

### Visit http://localhost:8080 to interact with your PDF chatbot.