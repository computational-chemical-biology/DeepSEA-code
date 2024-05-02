# DeepSEA-code

A guide to reproduce [DeepSEA](https://github.com/tiagocabralborelli/DeepSEA-project) analysis 


Primary data were obtained from the following works
1. [HMD-ARG: hierarchical multi-task deep learning for annotating antibiotic resistance genes](https://microbiomejournal.biomedcentral.com/articles/10.1186/s40168-021-01002-3)

2. [NCRD: A non-redundant comprehensive database for detecting antibiotic resistance genes](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC10590964/)

**Repository files map**
```
DeepSEA-code:
    data: complete data used in project
        benchmarking: protein sequences from holdout test data and result from benchmarked tools
        HMD:  AMR sequences, datasets and encoders for all models fitted for this work 
        NCRD: AMR sequences, datasets and encoders for all models fitted for this work 
        pseudo: pseudo proteins sequences, scrips to get sequences and construct the pseudo data
        real: real genomes used in DeepSEA evaluation
            ccbl: BRA006 genome from our prior work 
            dantas: TDases sequences found by HMMs
            refseq: proteins from reference genomes retrivied from SKAPE patogens
        uniprot: proteins non related to AMR download from Uniprot/Swisprot database
    models: all models used
    notebooks: jupyter notebooks used in this project
        GridSearch.ipynb: code used to hyperparameters optimization 
        BestModelTrain.ipynb: code to fit models using the best hyperparameters
        BestModelEval.ipynb: evaluation of fitted models on the hould out test set
        Embedding.ipynb: Code to plot t-SNEs from GlobalAveragePooling layer matrices
        Database.ipynb: database barplots
        TestOnGenomes.ipynb: evaluation on real data from SKAPE genomes
        TestOnPseudo.ipynb: evaluation on simulated data
        TDases: evaluation on proteins found by HMMs 
    
```

