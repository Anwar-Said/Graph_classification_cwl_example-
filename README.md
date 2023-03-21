# Graph Classification CWL Example
This repository include a cwl example for graph classification task. The cwl workflow contains three components: FileInput, model and results. 

**Input**: The input of the model is a molecular dataset which contains 188 toxic and non-toxic compounds in a networkx format. This dataset is known as MUTAG and available on PyG (https://www.pyg.org).
**Graph Descriptor**: This module uses NetLSD (https://arxiv.org/abs/1805.10712), a spectral graph descriptor that transfrom the dataset into a d dimensional space. 

**Classifier**: Random Forest is used for the classification. 

# Running the workflow

**Build Docker**: 

git https://github.com/Anwar-Said/Graph_classification_cwl_example-.git

cd Graph_classification_cwl_example- </br>


**run command**: docker build -t gc_docker:latest . </br>

cd GC_toxicity
```
cwltool --no-match-user --no-read-only --preserve-environment LEAP_CLI_DIR GC_toxicity.cwl.json --FileInput data/dataset.pkl
```






