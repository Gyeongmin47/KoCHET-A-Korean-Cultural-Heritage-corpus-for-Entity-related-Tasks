<div align="left">

# KoCHET: A Korean Cultural Heritage corpus for Entity-related Tasks [Accepted at COLING 2022]

[![Paper](https://img.shields.io/badge/Paper-ACL_Anthology-red)](https://aclanthology.org/2022.coling-1.308/)
[![Conference](https://img.shields.io/badge/COLING-2022-crayon)](https://coling2022.org/)
[![Demo](https://img.shields.io/badge/Demo-KoCHET-orange)](http://nlplab.iptime.org:9079/)


We propose :kr: _**KoCHET dataset v 1.0**_ :kr: Korean cultural heritage corpus for entity-related tasks, named entity recognition (NER), relation extraction (RE), and entity typing (ET).

This research was conducted within the framework of the project "_Development of Intelligent Curation and Service Platform-based Digital Asset for Immersive Cultural Heritage_" presented in the South Korean Ministry of Culture.

- Official paper: [https://aclanthology.org/2022.coling-1.308/](https://aclanthology.org/2022.coling-1.308/)
- Web demo is available here! :grin: : [![Demo](https://img.shields.io/badge/Demo-KoCHET-orange)](http://nlplab.iptime.org:9079/)

</div>

------------------------------------------
## :mag_right: Download 

KoCHET is uploaded ***[**here**](https://drive.google.com/drive/folders/1E-jAQ8wmoPFRNJAtBPfya1KyK3jUq3XS?usp=sharing)***

------------------------------------------
## :open_file_folder: ***Folder Description***

- ```KoCHET Directory Link```: 

```
KoCHET - a Korean cultural heritage corpus
  ├─ Named Entity Recognition (NER):
                                ├─ ner_{train,dev,test}.json
                                ├─ coarse_list.txt
  ├─ Relation Extraction (RE):
                          ├─ re_{train,dev,test}.json
                          ├─ relation_list.txt
  ├─ Entity Typing (NER):
                    ├─ et_{train,dev,test}.json
                    ├─ fine_grained_list.txt
```

- License: **KoCHET** is intended for non-commercial research purpose only.


------------------------------------------
## :bookmark_tabs: ***Dataset Statistics***

| Task |                |  Train  |   Dev  |  Test  |
|:----:|:--------------:|:-------:|:------:|:------:|
|  NER | # of examples  |  89,884 | 11,245 | 11,233 |
|      | # of entities  | 393,076 | 32,003 | 32,153 |
|  RE  | # of examples  |  31,012 |  3,876 |  3,877 |
|      | # of relations |  64,080 |  8,031 |  7,831 |
|  ET  | # of examples  |  90,558 | 11,320 | 11,320 |
|      | # of mentions  | 266,209 | 33,226 | 33,395 |


------------------------------------------
## :bookmark_tabs: ***Baseline***

|                     |       NER       |                 |               |               |    RE     |           |    ET     |           |
|:-------------------:|:---------------:|:---------------:|:-------------:|:-------------:|:---------:|:---------:|:---------:|:---------:|
|        Model        | Entity F1 macro | Entity F1 micro | Char F1 macro | Char F1 micro | F1 macro  | F1 micro  | F1 macro  | F1 micro  |
| `mBERT`             |      59.81      |      58.99      |     71.80     |     90.44     |   80.85   |   89.94   |   91.64   |   91.60   |
| `XLM-RoBERTa-base`  |    **76.57**    |    **79.67**    |   **82.69**   |   **94.77**   |   80.29   |   89.79   |   91.13   |   91.00   |
| `KLUE-BERT-base`    |      39.31      |      33.40      |     55.63     |     81.06     | **82.44** |   90.77   | **93.08** | **93.02** |
| `KLUE-RoBERTa-base` |      38.92      |      33.48      |     55.47     |     81.08     |   82.42   | **90.78** |   92.80   |   92.84   |


------------------------------------------
## Citation

:thumbsup: Please cite our paper in any published work that uses any of these resources. :thumbsup:

~~~bibtex
@inproceedings{kim-etal-2022-kochet,
    title = "{K}o{CHET}: A {K}orean Cultural Heritage Corpus for Entity-related Tasks",
    author = "Kim, Gyeongmin  and
      Kim, Jinsung  and
      Son, Junyoung  and
      Lim, Heuiseok",
    booktitle = "Proceedings of the 29th International Conference on Computational Linguistics",
    month = oct,
    year = "2022",
    address = "Gyeongju, Republic of Korea",
    publisher = "International Committee on Computational Linguistics",
    url = "https://aclanthology.org/2022.coling-1.308",
    pages = "3496--3505",
    abstract = "As digitized traditional cultural heritage documents have rapidly increased, resulting in an increased need for preservation and management, practical recognition of entities and typification of their classes has become essential. To achieve this, we propose KoCHET - a Korean cultural heritage corpus for the typical entity-related tasks, i.e., named entity recognition (NER), relation extraction (RE), and entity typing (ET). Advised by cultural heritage experts based on the data construction guidelines of government-affiliated organizations, KoCHET consists of respectively 112,362, 38,765, 113,198 examples for NER, RE, and ET tasks, covering all entity types related to Korean cultural heritage. Moreover, unlike the existing public corpora, modified redistribution can be allowed both domestic and foreign researchers. Our experimental results make the practical usability of KoCHET more valuable in terms of cultural heritage. We also provide practical insights of KoCHET in terms of statistical and linguistic analysis. Our corpus is freely available at https://github.com/Gyeongmin47/KoCHET.",
}

~~~

:email: If you have any questions / comment related to this work, please do not hesitate to contact the authors: Gyeongmin Kim <totoro4007@korea.ac.kr>, Jinsung Kim <jin62304@korea.ac.kr>, Junyoung Son <s0ny@korea.ac.kr>.
