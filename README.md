## <p align="center">Extractive Summarization based on word frequency using Spacy </p>

Aim of this project is to showcase how to formulate a crisp summary of any document or article with **words/sentences importance**. Started with word level importance using their weights, followed by sentence level where these weights were aggregated to determine sentence level importance. 

#### Follow the instructions below: 
New to conda?? a **useful guide** - https://conda.io/projects/conda/en/latest/user-guide/getting-started.html
```
conda activate <virtual_environment_name>
```
Alternatively, for MAC and linux/unix platforms, there is an easy way to create the virtual environment as below - 
```
python -m venv venv && source venv/bin/activate
```

Install all the requirements(requisite packages) - quick way to do it by using the below command: 
```    
python -m pip install -r requirement.txt
```
Open jupyter notebook from the conda environment (run locally and you can use chrome/edge/IE etc. browsers, to open jupyter notebook and python files)

```Open extractive_summarization.ipynb```

This is an step by step guide for extractive summarization. go thru the comments to know more about the approach. 

#### Validation metric: ROUGE

This is still an area of potential research to validate text generation. However, ROUGE (Recall-Oriented Understudy for Gisting Evaluation) score will give an approximate measure to check the results w.r.t. target summary.

#### Future work:

Implemented **TestRank and PageRank** algorithm together, to find significant sentences, to generate the summary-
- TestRank helps by creating the graph where **nodes represent the 'sentences' and edges 'the similarity' between them**. 
- PageRank algorithm helps in **sorting these sentences from high to low importance range**. Thereafter, pick TOP-N sentences to summaries the document (Can specify number of words as well to genearate the summary) 
