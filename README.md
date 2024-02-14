# (I am working on a research paper with this paper as one of the main references and hence am documenting my edits and changes here)

# AttentionSiteDTI
[![PWC](https://img.shields.io/endpoint.svg?url=https://paperswithcode.com/badge/attentionsitedti-an-interpretable-graph-based/drug-discovery-on-bindingdb)](https://paperswithcode.com/sota/drug-discovery-on-bindingdb?p=attentionsitedti-an-interpretable-graph-based)

This is The repository for supporting matterial of "AttentionSiteDTI: an interpretable graph-based model for drug-target interaction prediction using NLP sentence-level relation classification"
https://academic.oup.com/bib/advance-article/doi/10.1093/bib/bbac272/6640006

![AttentionSiteDTI](AttentionSiteDTI.png)

## Requirements
A suitable [conda](https://conda.io/) environment can be created:
```
conda env create -f noveldti.yml
conda activate noveldti
```
## Data
All data used in this paper are publicly available and can be accessed here: [DUD-E](http://dude.docking.org ), [BindingDB-IBM dataset](https://github.com/IBM/InterpretableDTIP), [Human dataset](https://github.com/masashitsubaki/CPI_prediction/tree/master/dataset) and [human sequence to pdb](https://github.com/prokia/drugVQA/tree/master/data)

## Demo Instructions
After downloading the human dataset you and place it in the project root folder you can generate the preprocessed data by running
```
python human_data.py
```
After generating the human_part_train.pkl, human_part_val.pkl and human_part_test.pkl you can start training the model by running
```
python main2.py
```
# Cite
If you find this repo to be useful, please cite our paper. Thank you.
```
@article{yazdani2022attentionsitedti,
  title={AttentionSiteDTI: an interpretable graph-based model for drug-target interaction prediction using NLP sentence-level relation classification},
  author={Yazdani-Jahromi, Mehdi and Yousefi, Niloofar and Tayebi, Aida and Kolanthai, Elayaraja and Neal, Craig J and Seal, Sudipta and Garibay, Ozlem Ozmen},
  journal={Briefings in Bioinformatics}
}
```




