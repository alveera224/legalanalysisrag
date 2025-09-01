# Legal Analysis Assistant
A chatbot to help you navigate EU AI regulation in a friendly way.

This is a RAG system implementation, using:
- LLM - GPT-4o
- VectorDB - ChromaDB
- Embedding functions - OpenAI
- Agents - LangChain 

It demonstrates how efficient this type of system can be for big documents as context and how well the LLM understands legal terms.

For the purpose of this demo, the context is The Artificial Intelligence Act, adopted by the EU Parliament on 13 March 2024. The system can be extended to other legal papers. 

### Installing
After cloning the repository, set your OpenAI API key as an environment variable named `OPENAI_API_KEY`.
```bash
export OPENAI_API_KEY=your_key_value_here
```
To run it locally, from the `legalai` folder use:
```bash
streamlit run app.py
```

### Notes
- The first run will download/process the EU AI Act and create a local ChromaDB store.
- Ensure `OPENAI_API_KEY` is set before asking questions in the UI.
