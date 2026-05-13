# IMORNpred: Prediction of Immunomodulatory Potential of RNA Sequences

Welcome to the official documentation for **IMORNpred**, a computational method developed for predicting the immunomodulatory potential of single-stranded RNA (ssRNA) sequences. This tool is designed to assist researchers in designing non-toxic siRNAs and potent RNA-based vaccine adjuvants by identifying whether an RNA sequence will activate or evade the innate immune system.

**Web Server:** [http://crdd.osdd.net/raghava/imornpred/](http://crdd.osdd.net/raghava/imornpred/)(https://webs.iiitd.edu.in/raghava/imrna)

---

## Citation

Chaudhary, K., Nagpal, G., Dhanda, S. K., & Raghava, G. P. S. (2016). 
**Prediction of Immunomodulatory potential of an RNA sequence for designing non-toxic siRNAs and RNA-based vaccine adjuvants.** *Scientific Reports*, 6, 20678. 
[https://doi.org/10.1038/srep20678](https://doi.org/10.1038/srep20678)

---

## About the Platform

The innate immune system recognizes foreign RNA through pattern recognition receptors like Toll-like receptors (TLRs). While this effect is desirable for vaccine adjuvants and immunotherapy, it causes unwanted immunotoxicity in siRNA-based therapies. IMORNpred allows for the design of RNA sequences with specific immunomodulatory potentials to suit these different therapeutic needs.

### Dataset Overview
The models were trained and validated on a high-quality dataset:
* **Immunomodulatory Oligoribonucleotides (IMORNs)**: 602 experimentally verified ssRNA sequences (length 17–27 nucleotides).
* **Non-immunomodulatory Sequences**: 520 circulating miRNAs.

---

## Key Features

### Prediction and Design
* **Potency Prediction**: Predicts whether an ssRNA sequence is immunomodulatory or non-immunomodulatory.
* **Mutant Generation**: Helps users design RNA analogs with altered immunomodulatory effects by suggesting specific nucleotide substitutions.
* **Feature Analysis**: Utilizes various features including nucleotide composition, transition, and distribution to achieve high prediction accuracy.

### Performance Metrics
The models were evaluated using five-fold cross-validation and external validation:
* **Maximum Accuracy**: Achieved a maximum accuracy of 83.21%.
* **Matthews Correlation Coefficient (MCC)**: Achieved a maximum MCC of 0.66.

---

## Technical Overview

IMORNpred leverages diverse RNA features and machine learning algorithms to model the immunomodulatory potential of sequences.

* **Machine Learning**: Developed using Support Vector Machines (SVM) and other classifiers like Random Forest and K-Nearest Neighbor.
* **Input Features**: Includes simple composition, binary profiles, and hybrid features combining multiple descriptors.
* **Motif Discovery**: Analysis of preferred motifs (e.g., "UGU", "GUGU") that contribute significantly to the immunomodulatory nature of RNA.

---

## Applications

* **siRNA Therapeutics**: Designing "stealth" siRNAs that avoid triggering an innate immune response to prevent toxicity.
* **Vaccine Adjuvants**: Identifying potent RNA sequences that can act as adjuvants to enhance the efficacy of vaccines.
* **Immunotherapy**: Discovering IMORNs that can be used to specifically modulate the immune system for treating various diseases.

---

## Contact & Authors

**Prof. Gajendra P. S. Raghava**
Department of Computational Biology, Indraprastha Institute of Information Technology (IIIT-Delhi), New Delhi, India.
**Email**: raghava@iiitd.ac.in / raghava@imtech.res.in

---

## License

This resource is open-access and distributed under the terms of the **Creative Commons Attribution 4.0 International License**, permitting unrestricted use and distribution provided the original work is properly credited.
