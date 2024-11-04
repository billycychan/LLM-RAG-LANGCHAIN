
# Local RAG LnagChain

This repository contains a Jupyter Notebook demonstrating a local Retrieval-Augmented Generation (RAG) pipeline. 
The notebook shows how to load documents, embed them into a vector store, and perform similarity-based retrieval. 
This setup can be useful for applications such as question-answering systems, knowledge-based search, and document analysis.

## Notebook Contents

The notebook, `LLM RAG Demo.ipynb`, is organized into the following sections:

1. **Document Loading**: 
   - Loads a PDF document using the `PyPDFLoader` from LangChain.
   - Splits the loaded text into manageable chunks using `RecursiveCharacterTextSplitter`, allowing for efficient processing during retrieval.

2. **Vector Store Initialization**:
   - Initializes a vector store with `Chroma`, a vector database for managing embeddings.
   - Uses `OllamaEmbeddings` with the `nomic-embed-text` model to embed the document chunks.

3. **Query Processing and Retrieval**:
   - (Likely includes, or you can add) a process to query the vector store to retrieve relevant document sections based on user input.

## Requirements

To run this notebook, you will need the following dependencies:

- Python 3.x
- [LangChain](https://github.com/hwchase17/langchain)
- [Chroma](https://github.com/chroma-core/chroma)
- Other dependencies as specified in the notebook, such as embedding models

You can install the necessary packages using:

```bash
pip install langchain chroma
```

## Usage

1. **Load Documents**: Place your PDF files in the specified directory and update the file path in the notebook if needed.
2. **Run the Notebook**: Execute each cell sequentially to load the document, initialize embeddings, and perform retrieval.
3. **Customize**: You can modify the text splitter parameters or the embedding model based on your specific use case.

## Acknowledgements

This demo relies on open-source libraries, particularly LangChain for document loading and Chroma for managing embeddings.

---

Feel free to reach out with any questions or suggestions for improvement!
