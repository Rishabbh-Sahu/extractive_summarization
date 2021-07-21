## Extractive Summarization based on word frequency using Spacy

Aim of this project is to showcase how using word and sentence importance, we can formulate a crisp summary of any document or article. Started with word level importance and their weights, followed by sentence level where these weights were aggregated to determine sentence level importance. 

#### Follow the instructions below: 

conda activate <virtual_environment_name>

Install all the requirements(requisite packages) -  
    quick way to do it by using the below command: 
    
    python -m pip install -r requirement.txt

Open jupyter notebook from the conda environment (run locally and you can use chrome, edge etc browser to open jupyter notebook, python files)

Open extractive_summarization.ipynb

This is an step by step guide for extractive summarization. go thru the comments to know more about the approach. 

#### Validation metric - ROUGE

This is still an area of potential research to validate text generation. However, ROUGE score will give an approximate measure to check the approach w.r.t. target summary.

#### Future work - 

Implementing TestRank and PageRank algorithm together to find significant sentences to generate the summary. TestRank helps by creating the graph where nodes represent the sentences and edges similarity between the sentences. Then, PageRank algorithm helps in sorting these sentences from high to low importance range. Thereafter, pick TOP-N sentence to summaries the document.

#### Model dependencies: 
Code has been written on window's 10 machine with 'miniconda', However it should work across operating systems. 
