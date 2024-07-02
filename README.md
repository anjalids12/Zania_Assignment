# Zania_Assignment
**Document based question answering system**

Following are steps that I used to build this project:

1. Text Extraction from each page of the PDF and stored into dataframe with its page number and page text.
2. Find the embeddings of each page using the pre-trained sentence-transformer model.
3. Find the embedding of the given question using the pre-trained sentence-transformer model.
4. Find the cosine similarity of the question embedding (got in 3) and each page embedding(got in 2).
5. Take the top 2 pages with high cosine similarity.
6. Pass these 2 pages and question using the proper prompt to get the answer.
