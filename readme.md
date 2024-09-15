
# Traceback: A Fault Localization Technique for Molecular Programs

This repository contains the artifacts for Traceback: A Fault Localization Technique for Molecular Programs, pressent at the 33rd ACM SIGSOFT International Symposium on Software Testing and Analysis.

## Reference

@inproceedings{  10.1145/3650212.3652138,   
author = {Gerten, Michael C. and Lathrop, James I. and Cohen, Myra B.},  
title = {Traceback: A Fault Localization Technique for Molecular Programs},  
year = {2024},  
isbn = {9798400706127},  
publisher = {Association for Computing Machinery},  
address = {New York, NY, USA},  
url = {https://doi.org/10.1145/3650212.3652138},  
doi = {10.1145/3650212.3652138},  
booktitle = {Proceedings of the 33rd ACM SIGSOFT International Symposium on Software Testing and Analysis},  
pages = {415–427},  
numpages = {13},  
keywords = {chemical reaction networks, fault localization, molecular programs, software debugging},  
location = {Vienna, Austria},  
series = {ISSTA 2024}  
}

## Acknowledgements

This material is based upon work supported by the National Science Foundation under Grant  CCF #1909688 and FET #1900716.

Disclaimer: “Any opinions, findings, and conclusions or recommendations expressed in this material are those of the author(s) and do not necessarily reflect the views of the National Science Foundation.”

## RQ1

RQ1/RQ1-LocalizationValues.csv contains the localization ranks and normalized ranks for the three methods (Species, Reaction, Traceback) in the case study. All subjects are evaluated, with each row being a crn program run. Each mutant program is ran 5 times.

## RQ2

RQ2/RQ2-LocalizationValues.csv contains the localization ranks and normalized ranks for the Traceback method in the case study. All subjects are evaluated, with each row being a mutant run with a listed test suite, Functional, Metamorphic, or Invariant.  The all test suite is the rows without a test suite label, which used all tests for the subject. Each crn program is ran 5 times.

RQ2/KW-Subject-TestType.pdf are the per subject and per test suite RQ3 results for varying k and w using the Traceback method.

The k-parameter and w-parameter tables are Table 6 from the paper with the standard deviation included in RQ2 directory.

## RQ3

RQ3/RQ3-LocalizationValues.csv contains the localization ranks and normalized ranks for the 3 methods (Species, Reaction, Traceback) in the case study. This file is over the paramter space of the Traceback method. Each row is a parameter selection, and was ran 5 times. We have the data for all subject crn programs in the study included.

RQ3/Mod_TestType-KW-Boxplots.pdf contains the effect of k and w on the normalized rank of the mod subject. Extended from Figure 8 in the submission.

## Subjects

The subject directory contains the six subjects used in the case study.
Each subject archive file has the models for each crn program used in the case study.
The archive also contain a TestMatrix.csv file which defines the abstract test properties and the inputs for each abstract test
and the InputMatrix.csv file contains what the initial values of the input species are for each input defined in TestMatrix.csv.
