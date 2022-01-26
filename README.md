# Why Did You Not Compare With That? Identifying Papers for Use as Baselines

This repository contains the supplementary material for the paper titled "Why Did You Not Compare With That? Finding Papers for Use as Baselines", accepted for publication at the [44th European Conference on Information Retrieval (ECIR 2022)](https://ecir2022.org/). A pre-print of the paper is available on [arXiv](https://arxiv.org/abs/2201.08089).

We used ACL Anthology Reference Corpus (ARC) [1] as the base data source for preparing the annotated dataset for our study. The ARC corpus consists of scholarly papers published at various Computational Linguistics up to December 2015. The corpus consists of 22; 875 articles and provides the original PDFs, extracted text and logical document structure (section information) of the papers, and parsed citations using the ParsCit tool [2]. 

The repository provides the annotated data for the baseline classification task. The main data file (baseline_labels.pkl) provides following information about the 2075 papers annotated by the human evaluators.

- ARC Corpus ID of the paper; 
- a list of all the references in the paper extracted by ParsCit;
- for each extracted reference, a binary label indicating whether the reference in the paper corresponds to a baseline or not. 1 indicates that the reference has been used as a baseline in the paper and 0 indicates a non-baseline reference.

**References**

1. Bird, S., Dale, R., Dorr, B.J., Gibson, B.R., Joseph, M.T., Kan, M.Y., Lee, D., Powley, B., Radev, D.R., Tan, Y.F.: The acl anthology reference corpus: A reference dataset for bibliographic research in computational linguistics. In: LREC. European Language Resources Association (2008)
2. Councill, I.G., Giles, C.L., Kan, M.Y.: Parscit: an open-source crf reference string parsing package. In: LREC. European Language Resources Association (2008)
