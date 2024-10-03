# MPP
Repository of resources on  Molecular Property Prediction ***(MPP)***.\
This project is associated with the survey paper ***"Advancements in Molecular Property Prediction: A Survey of Single and Multimodal Approaches"***
## Summary of datasets in MPP 🗂️
|**Property**| **Dataset**       | **Description** |**Reference**|
| -------|-------| ----------------------------------------------|-------|
| Solubility | [ESOL](https://moleculenet.org/datasets-1})| Contains chemical structures along with their corresponding experimentally determined solubility values in water|[Paper](https://academic.oup.com/bib/article/23/1/bbab367/6366324)|
| Solv. Energy | [FreeSolv](https://moleculenet.org/datasets-1})| provide chemical structures along with experimentally determined solvation free energy values | [Paper](https://onlinelibrary.wiley.com/doi/10.1155/2022/8464452)
| Hydrophobicity | [Lipophilicity](https://moleculenet.org/datasets-1})| depicts the tendency of a molecule to dissolve in lipids or non-polar solvents | [Paper](https://pubmed.ncbi.nlm.nih.gov/36526280)|
| Affinity | [BACE](https://moleculenet.org/datasets-1})| consists of molecules that are tested for their ability to inhibit the BACE enzyme, with associated experimental measurements of their inhibitory activity | [Paper](https://pubmed.ncbi.nlm.nih.gov/28696688) |
| Permeabiltiy | [BBBP](https://moleculenet.org/datasets-1})| contains molecular structures of compounds along with their experimentally measured blood-brain barrier permeability values|[Paper](https://pubmed.ncbi.nlm.nih.gov/36002937/)| 
| Toxicity | [Tox21](https://moleculenet.org/datasets-1}) | contains information on the biological activity of thousands of compounds across a panel of assays covering a range of biological processes and endpoints | [Paper](https://openreview.net/forum?id=xQUe1pOKPam) | 
| Toxicity | [Toxcast](https://moleculenet.org/datasets-1}) | includes results from various assays covering endpoints related to cytotoxicity, genotoxicity etc. and the biological activity of chemicals across them | [Paper](https://pubmed.ncbi.nlm.nih.gov/36526280/)| 
|Toxicity | [ClinTox](https://moleculenet.org/datasets-1}) | consists of molecular structures along with binary labels indicating whether each molecule is associated with toxicity or not | [Paper](https://www.sciencedirect.com/science/article/abs/pii/S0957417422020735)|
|Side-effects | [SIDER](https://moleculenet.org/datasets-1}) |  provides comprehensive coverage of adverse drug reactions (ADRs) associated with a wide range of drugs | [Paper](https://pubmed.ncbi.nlm.nih.gov/36526280/)|
| Quantum mechanics | [QM7](https://moleculenet.org/datasets-1}) | includes atomization energies and energies of the highest occupied molecular orbital (HOMO) for organic molecules | [Paper](https://arxiv.org/abs/1909.00259)|
| Bioactivity | [MUV](https://moleculenet.org/datasets-1}) | contains a set of molecules labeled as active (binders) or inactive (non-binders) with respect to the 17 different biological targets | [Paper](https://arxiv.org/abs/1709.03741)|
| Efficacy | [HIV](https://moleculenet.org/datasets-1}) | provide results from screening experiments aimed at identifying compounds with potential anti-HIV activity | [Paper](https://arxiv.org/abs/1709.03741)|
| Cardiotoxicity | [hERG blocking](https://github.com/zhaoqi106/DMFGAM) | contains information about the inhibition activity of compounds against the hERG potassium ion channel  | [Paper](https://pubmed.ncbi.nlm.nih.gov/36584603/)|
| Mutagenicity | [Ames data](https://pubs.acs.org/doi/10.1021/ci300400a) | contains structural information and experimental results for a large number of chemical compounds tested for their mutagenic activity | [Paper](https://pubmed.ncbi.nlm.nih.gov/34555723/) | 
| Mutagenicity | [Hansen data](https://pubs.acs.org/doi/abs/10.1021/ci900161g) | contains SMILES and experimental results for a large number of chemical compounds tested for their mutagenic activity | [Paper](https://jcheminf.biomedcentral.com/articles/10.1186/s13321-021-00541-z)|




## Descriptor calculation packages/servers 📦 | 🖥️ 
|**Package/Server**| **Descriptors** |**Count**  | **Type** |**Acess Link**|
| -------|------------| ---------------------- |---------------------- |-------------------|
|Mordred |1826 descriptors|643|2D and 3D |[Link](https://pypi.org/project/mordred)|
| Chemdes|3679 descriptors, 59 fingerprints|264| 1D, 2D and 3D|[Link](www.scbdd.com/chemdes)|
| PaDELpy|1875 descriptors, 12 fingerprints|2258| 1444 1D, 2D, and 431 3D|[Link](http://www.yapcwsoft.com/dd/padeldescriptor)|
|  CDK\_pywrapper|- |- |1D, 2D, 3D descriptors and fingerprints|[Link](https://pypi.org/project/CDK-pywrapper/)|
| pybel |-| 408 |1D, 2D descriptors |[Link](https://pypi.org/project/pybel/)|
| PyBioMed|775 descriptors, 19 fingerprints| 112 |1D, 2D, 3D descriptors |[Link](http://projects.scbdd.com/pybiomed.html)|
|Rcpi|>300 molecular descriptors and 10 fingerprints|130 |1D,2D Descriptors |[Link](http://bioconductor.org/packages/release/bioc/html/Rcpi.html)|
|Biotriangle|540 descriptors and 7 fingerprints | 47| 1D, 2D descriptors| [Linl](http://biotriangle.scbdd.com)|
## Expert-crafted feature based approaches  🔧
|**Year**| **Dataset** | **Task** | **Input Representation** | **Method** |**Evaluation criteria**|**Reference**|
| -------|------------| ---------------------- |--------|---------|----------|-------------|
|2017 |AMES | Classification|  Descriptors, ECFP-14 | Naive Bayes | 5-Fold CV |[Link](https://pubmed.ncbi.nlm.nih.gov/28232239/) |
|2018| eChemPortal | Classification| Descriptors,PubChem, MACCS,Substructure, CDK,Estate | SVM,KNN,Naive Bayes,DT,RF,ANN | 5-Fold CV |[Link](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC6062245/) |
|2018 | BBBP | Classification | Descriptors,PubChem, KlekotaRoth,CDK-Extended, 2D-Atom Path,FP4 | SVM | Train-Test Split |[Link](https://pubmed.ncbi.nlm.nih.gov/29564576/) |
|2018|BBBP|Classification | Descriptors,Fingerprints |LR,RF,KNN,SVM,MLP |10-Fold CV|[Link](https://pubmed.ncbi.nlm.nih.gov/30110511/) |
|2018 | ADME| Classification, Regression|ECPF-3 |DNN, SVM | 10-Fold CV |[Link](https://pubmed.ncbi.nlm.nih.gov/30586300/)  |
|2019 |𝐿𝑜𝑔𝐷7.4 |Classification| Multiple Descriptors |Consensus of RF, XG-boost,SVM,GB| Random Split| [Link](https://pubmed.ncbi.nlm.nih.gov/31869226/) |
|2021 |OECD-TG471| Classification |Fingerprints| Balancing Techniques,GBT,RF, SVM, MLP,KNN| Random Split| [Link](https://www.sciencedirect.com/science/article/pii/S2468111321000268) |
|2022 |BBBP |Classification| Mol2Vec |1D-CNN, MLP |10-Fold CV| [Link](https://onlinelibrary.wiley.com/doi/abs/10.1002/minf.202100315)  |
|2022|HIV,BACE,QM7,Lipo, BBBP,ESOL etc.|Classification,Regression| Descriptors,Fingerprints |RF |Random Split| [Link](https://chemistry-europe.onlinelibrary.wiley.com/doi/abs/10.1002/cphc.202200255) |





## SMILES-based methods
|**Year**| **Dataset**    |**Code/Server**   |**Reference**|
| -------|------| ---------------------- |------|
|2019|BBBP, BACE, Ames, ESOL|[GitHub](https://github.com/jrwnter/cddd) |[Paper](https://pubs.rsc.org/en/content/articlelanding/2019/sc/c8sc04175j)|
|2019|PubChem|-|[Paper](https://arxiv.org/pdf/2404.03969)|
|2020|Lipo, FreeSolv, HIV, BBBP|- |[Paper](https://jcheminf.biomedcentral.com/articles/10.1186/s13321-020-00430-x)|
|2020|Lipo, BACE, FreeSolv, BP, HIV, AMES, BBBP, ToxCast|[GitHub](https://github.com/bigchem/transformer-cnn)|[Paper](https://jcheminf.biomedcentral.com/articles/10.1186/s13321-020-00423-w)|
|2020|HIV, BACE, BBBP, Tox21, ClinTox, SIDER|-|[Paper](https://arxiv.org/pdf/1712.02034)|
|2021|Tox21, HIV, BBBPS, SIDER, CLINTOX| [GitHub](https://github.com/arwhirang/sa-mtl)|[Paper](https://arxiv.org/pdf/2010.11272)|
|2021|CLINTOX, QSAR datasets|[GitHub](https://github.com/XinhaoLi74/SmilesPE) |[Paper](https://pubs.acs.org/doi/10.1021/acs.jcim.0c01127)|
|2021|Tox21, BBBP, CLINTOX, SIDER|[GitHub](https://github.com/cxfjiang/MolBERT) |[Paper](https://onlinelibrary.wiley.com/doi/10.1155/2021/7181815)|
|2022|logS, logP, logD|[GitHub](https://github.com/EBjerrum/SMILES-enumeration) |[Paper](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC8912091/)|
|2022|Lipo, BACE, ESOL, HIV, FreeSolv|- |[Paper](https://www.sciencedirect.com/science/article/pii/S009813542100377X)|
|2022|HBV, HepG2|[GitHub](https://github.com/NTU-MedAI/S2DV)|[Paper](https://pubmed.ncbi.nlm.nih.gov/35062019/)|
|2022|MoleculeNET|- |[Paper](https://jcheminf.biomedcentral.com/articles/10.1186/s13321-022-00650-3)|
|2023|MoleculeNET, Cytotoxicity|[GitHub](https://github.com/PaccMann/chemical_representation_learning_for_toxicity_prediction)|[Paper](https://pubs.rsc.org/en/content/articlelanding/2023/dd/d2dd00099g)|
|2024|ESOL, FreeSolv, Lipo,BBBP, Clintox|-|[Paper](https://www.sciencedirect.com/science/article/pii/S0009250923010278)|


## GNN-based methods
|**Year**| **Dataset**   |**Code/Server**   | **Reference**|
| -------|------------|--------- |------------| 
|2019 |QM9, MUTAC, NCI1|-|[Paper](https://arxiv.org/abs/1905.11136)| 
|2019 |ChemBL|[GitHub](https://github.com/choderalab/gimlet)|[Paper](https://arxiv.org/abs/1909.07903)| 
|2019 |QM9, COD, CSD|-|[Paper](https://www.nature.com/articles/s41598-019-56773-5)|  
|2019|MUTAC|-|[Paper](https://arxiv.org/abs/1904.05811)| 
|2019 |ESOL, LIPO, Tox21|-|[Paper](https://www.researchgate.net/publication/340056095_Property_Prediction_of_Molecules_in_Graph_Convolutional_Neural_Network_Expansion)| 
|2019|HIV, MUV, BBBP, Tox21, SIDER, QM8, ESOL, LIPO|-|[Paper](https://pubmed.ncbi.nlm.nih.gov/31408336/)| 

## Multimodality-based methods
|**Year**| **Dataset** |I/P Modality   |**Code/Server**   | **Reference**|
| -------|------------|------|------------| ---------------------- |
| || || |
| || || |
| || || |

