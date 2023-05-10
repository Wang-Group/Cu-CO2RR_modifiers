# Cu-CO2RR_modifiers
This repository contains the raw data and machine learning codes used in our paper entitled "Modifiers Tuning C2+ Selectivity in CO2 Electroreduction by Reduction Potential: Combining Data-driven Machine Learning and Hypothesis-driven Experimentation."  

Codes
The following Jupyter notebooks contain the codes used for this study:  

1.Comprehensive Molecular Featurizer V5.0.ipynb: Generates the feature matrix, including Local Functional Group Fingerprint (LoFFi) and LoFFi-MOE features developed by Yuming Su and Yangtao Chen. An auxiliary file, "loffi.txt," is required for the precise and accurate definition of each functional group in SMARTS format.  
2.Classification-Multimodel_classifier.ipynb: Initial machine learning step containing 8 different models.  
3.Classification-GBCT-RecursiveFeat.ipynb: Implements recursive feature selection using the method provided by Scikit-learn.  

Raw Data
From 59 research papers published (before Mar, 2023) reporting the use of Cu catalysts with organic modifiers for CO2RR, we selected 33 papers that included the CO2RR activity of bare Cu as a control sample. We collected 237 experimental data points detailing the enhancement of CO2RR by adding different organic modifiers.  
1.CO2RRMolecularModification-HXR-20230323.xlsx: Contains data directly extracted from papers, including Faraday efficiency of reference Cu with and without modifiers, experimental conditions and DOI info.  
2.CO2RRmolecular_processeddata-20230328.xlsx: Presents calculated delta-FE values while retaining experimental conditions.  
3.Featurematrix_242_195.csv: Generated using "Comprehensive Molecular Featurizer V5.0.ipynb" by providing the 'smiles' and 'delta-FEC2+' columns from the "CO2RRmolecular_processeddata-20230328.xlsx" file as input.  
