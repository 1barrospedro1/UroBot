# UroBot
Urology-informed Large Language Model

UroBot is an advanced urology-specialized chatbot designed to enhance medical question-answering by leveraging the capabilities of large language models (LLMs) like GPT-3.5, GPT-4, and GPT-4o from OpenAI. Utilizing retrieval augmented generation (RAG) and the latest 2023 European Association of Urology (EAU) guidelines, UroBot aims to deliver accurate and explainable responses to urological board questions. In a comprehensive evaluation involving 200 European Board of Urology (EBU) In-Service Assessment (ISA) questions, UroBot-4o achieved a mean Rate of Correct Answers (RoCA) of 88.4%, significantly surpassing the performance of GPT-4o and typical urologists, with high consistency. You can run this with different guidelines.

### How to Run the UroBot Flask App Locally

1. **Set Up the Environment With Conda**:
   - Create a conda environment using the `environment.yml` file:
     ```bash
     conda env create -f environment.yml
     conda activate your_env_name
     ```

2. **Used With Ollama**: 
   - Install Ollama
   - Run:
     ```bash
     ollama pull qwen2.5:1.5b
     ollama pull granite-embedding:278m
     ```


3. **Run the Flask App**:
   - Execute the following command to start the application:
     ```bash
     flask --app UroBot_flask_app.py run
     ```
    
#### Citation

Martin J. Hetz, Nicolas Carl, Sarah Haggenmüller, Christoph Wies, Jakob Nikolas Kather, Maurice Stephan Michel, Frederik Wessels, Titus J. Brinker: Superhuman Performance on Urology Board Questions Using an Explainable Language Model Enhanced with European Association of Urology Guidelines
ESMO Real World Data and Digital Oncology 2024, DOI: https://doi.org/10.1016/j.esmorw.2024.100078
