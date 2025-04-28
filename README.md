**Extract Information from a Downloaded YouTube Transcript**

1.Install the dependencies

2.Download an example transcript from a YT video

3.Select the LLM model to use. (llama3 is downloaded)
Check the list of models available for Ollama here: https://ollama.com/library

4.Instantiate the model and the embeddings.

5.Load the transcription previously saved using TextLoader

6.Explit the document into chunks. If the transcript is very large, you might want to split it into chunks (because LLMs have input size limits).

7.Store the PDF in a vector space.(DocArrayInMemorySearch)
From Langchain docs:DocArrayInMemorySearch is a document index provided by Docarray that stores documents in memory. It is a great starting point for small datasets, where you may not want to launch a database server.

8.Instantiate the parser

9.Generate the conversation template
