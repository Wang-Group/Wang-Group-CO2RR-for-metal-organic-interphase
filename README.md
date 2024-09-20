This repository contains the raw data and machine learning codes used in our paper entitled 'Observation of Metal-Organic Interphase in Cu-based Electrochemical CO2-to-Ethanol Conversion' 
Codes The following Jupyter notebooks contain the codes used for this study:

**1. Factor analysis and analyze SHAP results.ipynb**: The extracted molecular fingerprint feature fragments were analyzed for correlation coefficients, and the columns with complete linear correlation were eliminated. The extracted physical and chemical properties of the molecules were analyzed for correlation coefficients, and the columns with complete linear correlation were eliminated. The reintegrated molecular fingerprints and the characteristics of the molecular physical and chemical properties were tested for correlation, and the physical and chemical properties of the molecules were subjected to factor analysis with the molecular fingerprint as input..According to the results of factor analysis, the SHAP analysis results of the Faraday efficiency of different products of CO2RR were factor-correlated.  
**2. Stepwise regression-FExx.ipynb**: Feature selection for FExx is performed using stepwise regression using methods provided by Scikit-learn. Codes were written for nine FE targets: H2, CO, CH4, C2H4, formate, acetate, EtOH, n-PrOH, and C2+ products.  
**3. Model metric-ROC curves-Confusion matrix-SHAP analysis-xx.ipynb**: According to the features screened by stepwise regression, the FE indicators of different classification models for each target product are output, including ROC curve, confusion matrix, accuracy, SHAP analysis, etc. Codes were written for nine FE targets: H2, CO, CH4, C2H4, formate, acetate, EtOH, n-PrOH, and C2+ products.
  
  **Raw data** are listed in the Supporting Information of the article, i.e., the CO2RR product data of all S-modified CuOx molecules and was arrange into **Target.csv** file on input.  
  
  1. **MFFmatrix-onlyS.csv**: Molecular fingerprint feature matrix input in factor analysis.  
  2. **Rdkitmatrix+sym descriptor-only S.csv**: Physical and chemical property characteristic matrix input in factor analysis.
  3. **updated_correlation_matrix_between_Original_and_Encoded_Features.csv and A1.csv**: The molecular fingerprint output during factor analysis is related to the characteristic matrix of the molecular physical and chemical properties.  
  
4. **Folder**: **20240611-S-体系-all metrics**: Contains the most important features extracted from the SHAP analysis for nine FE targets (H2, CO, CH4, C2H4, formate, acetate, EtOH, n-PrOH, and C2+ products) results for all CO2RR products written in csv files named 'shap_results-xx+
/MLP-top-features.csv' , used to correlate with the extracted factors.
  5. **Folder**: **S-体系-逐步回归挑选出来的特征**: Contains the selected features for nine FE targets (H2, CO, CH4, C2H4, formate, acetate, EtOH, n-PrOH, and C2+ products) results written in csv files named 'Selected_features-xx' for all CO2RR products by Stepwise regression.

The packages and versions installed in the runtime environment are as follows:  

  
