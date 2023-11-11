# Semantic Search
Semantic Search is a type of search technique which takes into consideration of the contents of the query rather than a lexical word comparison.

- The overall idea is that the data of the contents to be searched for are converted into word embeddings and it will be stored in the latent space based on the similarity of the contents.
- When a query is asked by the user, the query is converted into embeddings and the a nearest neighbour algorithm is used to identify the closed match with the query from the word embeddings space.
