# Cu-CO2RR_modifiers
This is a packup repository to share collected raw data and machine learning codes of paper named 
"Modifiers Tuning C2+ Selectivity in CO2 Electroreduction by Reduction Potential: Combining Data-driven Machine Learning and Hypothesis-driven Experimentation"

Codes:
All codes were written in jupyter notebook.
1.Comprehensive Molecular Featurizer V5.0.ipynb: generate Feature matrix. In this version we contain Local Functional group Fingerprint (LoFFi) and LoFFi-MOE features developed by Yuming Su and Yangtao Chen. An auxiliary file named "loffi.txt" is needed to consult precise and accurate defination of each functional group in SMARTS format.
2.Classification-Multimodel_classifier.ipynb: initially machine learning step containing 8 models.
3.Classification-GBCT-RecursiveFeat.ipynb: using Recursive feature selection method supported by sklearn to select feartures.

Raw data:
We found 59 research papers published (before Mar, 2023) that reported the use of Cu catalysts with organic modifiers for CO2RR. However, out of these papers, only 33 included the CO2RR activity of bare Cu as the control sample. 237 experimental data points were collected from these papers, which detailed the enhancement of CO2RR achieved by adding different organic modifiers.
1.CO2RRMolecularModification-HXR-20230323.xlsx: directly from papers, including Faraday efficiency of reference Cu with and without modifiers and experimental conditions.
2.CO2RRmolecular_processeddata-20230328.xlsx: delta-FE was calculated. Still containing experimental conditions.
3.Featurematrix_242_195.csv: Using two columns of data(smiles and delta-FEC2+) from CO2RRmolecular_processeddata-20230328.xlsx as input, "Comprehensive Molecular Featurizer V5.0.ipynb" was used to generated this csv.
