# genesys

Questo progetto e' solo un rapido test

## Appunti

- framework utilizzati:
  - [langchain](https://www.langchain.com/)
  - [ollama](https://ollama.ai) 

Cronostoria:
-  installazione git 
- installazione ollama
- installazione langchain
- avvio tutorial [quickstart](https://python.langchain.com/docs/get_started/quickstart)
  - step iniziale e' usarlo con open-ai
  - abbiamo visto come usare le chain di langchain
  - DZ: come faccio a tracciare a basso livello la chiamata per vedere cosa ha inviato alla API?
  - langchain_text_splitters e' sperimentale e richiede:
    ```bash
    pip install langchain-experimental
    ```
  - Questo snippet 
    ```python
    from langchain.chains import create_retrieval_chain

    retriever = vector.as_retriever()
    retrieval_chain = create_retrieval_chain(retriever, document_chain)
    ```
    genera questo errore

    ```
    ImportError: cannot import name 'SetupMode' from 'langchain_community.utilities.astradb' (/usr/local/lib/python3.11/site-packages/langchain_community/utilities/astradb.py)
    ```