## Workflow Summary

1. Download the documents

2. Get the hash id of each document, and append the id into the documents json file(A)

3. Use openai to generate up to 5 similar questions for each document, generate a json file(B) with id and questions

4. Based on B and A, create a list with the format [question, course, id] and write it into pd.df and then output it as csv.

