# SML-575
## Evaluating Information Retrieval Models using BERT features and OpenBookQA 

Dataset is present in : /scratch/pbanerj6/sml-dataset/ranking 
 
1. train.tsv 
2. val.tsv : Use this for model selection
3. test.tsv : Use this only for measuring accuracy and mrr

Embedding files contain tokens and their corresponding embeddings of size 768. 

Tasks:
1. Evaluate classifiers using only [CLS] tokens.
2. Evaluate using all tokens.



Tips to work on Jupyter in Agave:

1. Start an interactive session : interactive -n 20 
2. Note the host you start your session : "cg6-17"
3. source activate your_conda_env
4. pip install jupyterlab
5.1 unset XDG_RUNTIME_DIR
5.2 To start jupyter : jupyter lab --port=8889 --no-browser --ip=0.0.0.0 
Note the port 8889
6. You can run jupyter in nohup like : nohup jupyter lab --port=8889 --no-browser --ip=0.0.0.0 > jupyter.log &
7. Note the token generated in jupyter.log 
8. In another terminal/cmd prompt ssh to agave using port forwarding : ssh -L8889:localhost:8889 yourname@agave.asu.edu
9. In this new terminal/cmd prompt ssh to "cg6-17" using port forwarding : ssh -L8889:localhost:8889 yourname@cg6-17
10. In your browser open : localhost:8889. If a token is asked enter the token from jupyter.log




