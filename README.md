# masters-thesis
This repository contains the .pdf file of my master's thesis “Representing Evolving Knowledge Graphs through Incremental Embeddings”. 

This thesis addresses the lack of a benchmark for the assessment and comparison of incremental knowledge graph embedding models. 
Therefore I elaborated an evaluation framework which enables to examine incremental knowledge graph embedding models in-depth in context of an 
evolving knowledge graph but also allows to include static relatives into the comparison.

Further I compiled the datasets called Wikidata9M and WikidataEvolve which are sourced from the edit history of Wikidata. 
Wikidata9M can be found at https://github.com/rlafraie/Wikidata9M and describes the evolution of a knowledge graph represented by a time stream of fact insertions and deletions. 
WikidataEvolve manifests a transformation of Wikidata9M to provide data for the training and evaluation of incremental and static embedding models 
throughout the evolution of the knowledge graph.

Lastly, I implemented the incremental knowledge graph embedding technique Parallel Universe TransE (PuTransE) [1] to evaluate and compare it with the static embedding
technique of TransE [2] by using the constructed evaluation artefacts. The code of PuTransE has been implemented and integrated into the OpenKE framework [3]. 
The code can be found at my forked repository https://github.com/rlafraie/OpenKE. 
The experiments are persisted in corresponding folder https://github.com/rlafraie/OpenKE/tree/OpenKE-PyTorch/experiments.

## References
<a id="1">[1]</a> 
Yi Tay, Anh Tuan Luu, and Siu Cheung Hui. Non-parametric estimation of multiple embeddings for link prediction on dynamic knowledge graphs. In AAAI, pages 1243–1249. AAAI Press, 2017.

<a id="1">[2]</a> 
Antoine Bordes, Nicolas Usunier, Alberto García-Durán, Jason Weston, and Oksana Yakhnenko. Translating embeddings for modeling multi-relational data. In NIPS, pages 2787–2795, 2013.

<a id="1">[3]</a> 
Xu Han, Shulin Cao, Lv Xin, Yankai Lin, Zhiyuan Liu, Maosong Sun, and Juanzi Li. Openke: An open toolkit for knowledge embedding. In Proceedings of EMNLP, 2018.

