# running_llm_on_cpu_quantization
This project is a PDF-based Question Answering chatbot powered by a quantized version of LLaMA 2, efficient vector retrieval using FAISS, and a simple Flask web interface. Users can interact with their documents by asking questions, and the system will retrieve relevant content and generate accurate answers using local models—no internet or API key required!

How to Run?
🔹 Steps 1: Clone the Repository

git clone https://github.com/your-username/pdf-qa-chatbot.git
cd pdf-qa-chatbot

🔹 Steps 2: Create a Virtual Environment

conda create -n cpullama python=3.8 -y
conda activate cpullama
pip install -r requirements.txt

🔹Step 3: Download Quantized LLaMA 2 Model
Download the quantized model and place it in the model/ directory:

llama-2-7b-chat.ggmlv3.q4_0.bin

🔹 Step 4: Start the Application

python app.py

Visit http://localhost:8080 to interact with your PDF chatbot.

📁 Project Structure
📁 data/               # PDF documents
📁 model/              # Quantized LLaMA model file
📁 templates/          
 └── index.html        # Flask frontend
📁 src/
 └── helper.py         # Custom helper functions
app.py                 # Main Flask application
requirements.txt       # Python dependencies
README.md              # You are here!