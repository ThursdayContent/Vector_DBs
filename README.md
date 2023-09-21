
# Vector Databases

The project is about comparison of various Vector DBs and different types of similarity searches. This project also focusses on various installation steps & pre-requisites and issues encountered while installing the libraries.

OpenAI API is must to generate the embeddings from OpenAI. SentenceTransformer embeddings can also be used in place of OpenAI embeddings.
## Installation of Chromadb

Please run the following commands to install chromadb:

`pip install chromadb`

If Chromadb does not work after installation, please repeat the following steps:

    1. Install Microsoft Vc++ version > 14 
    2. Modify visual studio installer
    3. pip install more-itertools numba tiktoken==0.3.1

Github issues reference link fo Chromadb:
    https://github.com/chroma-core/chroma/issues/250

## Installation of Pinecone

To run Pinecone, the following APIs are must: 

    1. OpenAI API
    2. Pinecone API to be generated from https://www.pinecone.io/


Run the following to store Pinecone API in env: 

`pinecone.init(api_key="*****", environment="***")`

Please follow the following steps in case of SSL errors:

    1. Generate certifcate from Pinecone website.
    2. Add certificate in Manage Computer certifcate > Trusted root certification authorities from Windows start
    3. Proxy setup check if the Pinecone site is not reachable even after completion of above steps

Run the following command to update certificates

`python -m pip install --upgrade certifi`


## Link to the PDF

The PDF file used in the project can be downloaded from here:

https://www.fdic.gov/regulations/examinations/credit_card/pdf_version/ch2.pdf