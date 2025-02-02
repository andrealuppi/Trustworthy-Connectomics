#  Transitions between cognitive topographies: contributions of network structure, chemoarchitecture, and diagnostic categories.
Authors: A.I. Luppi, H.M. Gellersen, Z-Q. Liu, A.R.D. Peattie, A.E. Manktelow, R. Adapa, A.M. Owen, L. Naci, D.K. Menon, S.I. Dimitriadis & E.A. Stamatakis 

This repository provides the _Interactive Pipeline Selection Tool_ from Luppi et al., "Systematic evaluation of fMRI data-processing pipelines for consistent functional connectomics" Nature Communications (2024) ([published article](https://doi.org/10.1038/s41467-024-48781-5)).

The _Pipeline Selection Tool_ provides the results of systematically assessing 768 pipelines for obtaining a functional connectivity network from (preprocessed) functional MRI data.
The pipelines consist of all possible combinations of the following steps:
(i) Global signal regression (GSR or no GSR);
(ii) Definition of network nodes: AAL, Brainnetome, Glasser, Lausanne multi-scale anatomical (129, 234 or 463 nodes), Schaefer-Tian multi-scale functional (116, 232, or 454 nodes),
Independent Components Analysis (100, 200, or 300 components). 
(iii) Number of nodes: approximately 100, 200 or 300-400.
(iv) Edge definition: Pearson correlation or Mutual Information. 
(v) Edge filtering: pre-specified density (retaining 5%, 10%, or 20% of total edges, or matching the density of the structural connectome); pre-specified minimum weight (0.3 or 0.5);
or data-driven methods (Efficiency Cost Optimisation, and Orthogonal Minimum Spanning Trees).
(vi) Binary or weighted networks. 

Each pipeline is benchmarked against the following criteria:
**Criterion (I)**: Avoiding random test-retest differences.
**Criterion (II):** Detecting true experimental differences (reconfiguration induced by anaesthesia).
**Criterion (III):** Detecting inter-individual differences.
**Criterion (IV):** Avoiding systematic motion-induced differences.
**Criterion (V):** Producing non-empty networks.

Each criterion is assessed for each pipeline in four test-retest datasets (spanning ~1h, 2-4 weeks, 1-11 and 5-16 months) including different acquisition parameters and preprocessing/denoising (aCompCor and FIX-ICA).

The paper (available Open Access) provides a full description of each criterion and dataset.
To make this repository self-contained, a PDF _Guide to the Pipeline Selection Tool_ is also provided.

## Contact Information
For questions, please email: [al857@cam.ac.uk](al857@cam.ac.uk).

