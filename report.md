# Project Report: LLM-Powered Hotel Booking Analytics

## Implementation Choices

- **Model**: Used GPT-Neo or HuggingFace-compatible model for structured query extraction.
- **Embeddings**: Chosen `all-MiniLM-L6-v2` from `sentence-transformers` for fast and good semantic encoding.
- **Vector DB**: ChromaDB for in-memory document retrieval based on semantic similarity.
- **Framework**: Flask for serving APIs.

## Challenges

- **LLM hallucination**: Ensured consistent structured query extraction using deterministic decoding.
- **Data mismatch**: Handled incorrect date formats using pandas' robust parsing.
- **Colab limitations**: Used threading to run Flask within Google Colab.

## Output Validation

Queried using sample inputs and validated answers against expected aggregates.

## Future Work

- Add authentication layer.
- Support more query types and visualizations.
- Export analytics as downloadable reports.