# RSNA-MICCAI-Brain-Tumor-Radiogenomic-Classification

Gliobstoma is the most common form of brain cancer in adults and the one with the worst prognosis, with median survival being less than a year. The presence of a specific genetic sequence in the tumor known as MGMT promoter methylation has been shown to be a favorable prognostic factor and a strong predictor of responsiveness to chemotherapy.

Currently, genetic analysis of cancer requires surgery to extract a tissue sample. Then it can take several weeks to determine the genetic characterization of the tumor. 

**Aim is to develop a method to predict the genetics of the cancer through imaging (i.e., radiogenomics) that would potentially minimize the number of surgeries and refine the type of therapy required.**

Corresponding to each patient, there are 4 types of MRI sequences/modalities (T1w, T2w, T1wCE, FLAIR) and each of the modality can be in different orientation (Sagittal, Axial, Longitudnal) for different patients. So, we built 12 EfficientNet3D models, one for each type of sequence and orientation (eg: T1w Axial, T1w Longitudnal, T2w Axial etc.) 
For a given patient, since there are 4 modalities, we predicted the Methylation status of MGMT Promoter separately for each of the 4 modalities and then, finally averaged the four predictions in order to predict the MGMT promoter's methylation value.

Competition Link: https://www.kaggle.com/c/rsna-miccai-brain-tumor-radiogenomic-classification  
EfficientNet Weights: https://www.kaggle.com/datasets/yashikajain/effnetweights  
EfficientNet3D: https://www.kaggle.com/datasets/hihunjin/efficientnetpyttorch3d   
Kaggle Notebook: https://www.kaggle.com/yashikajain/efficientnet3d  
