# Assignment 5 Implementing a Simple Retrieval-Augmented Generation (RAG) System
# By Evelyn Bushell

## Models Used

### LLM Model
google/flan-t5-small

### Embedding Model
sentence-transformers/all-MiniLM-L6-v2

## Retrieval Process
The Knowledge Base is split into 5 chunks each with 300 characters. The retriever then compares the query with each chunk and grabs the chunks with the highest relevancy scores and adds them to the prompt.

## Results Analysis
This does seem to be very fact based. The model is extremely hesitant to provide an inaccurate answer and generally sticks to the context given to it, while still able to make obvious observations such as the chosen film being more sad than happy.