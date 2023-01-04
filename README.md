# Machine Learning for *In Situ* Photoluminescence Data of Perovskite Photovoltaics


This repository contains the code for the paper **"Process Insights into Perovskite Thin-Film Photovoltaics from Machine Learning with *In Situ* Luminescence Data"**(*add link*) and the corresponding dataset (*add link*).

## Reproducing the results

This repository contains all data and code needed to reproduce the results of the paper **"Process Insights into Perovskite Thin-Film Photovoltaics from Machine Learning with *In Situ* Luminescence Data"**.   

#### Repository Structure
```
├── README.md                                                           
├── requirements.txt                                - txt-file to install the environment
├── 00_extract_data_from_hdf5_file.ipynb            - Script to extract data from hdf5-file provided on Zenodo
├── 01_rationale_for_in_situ.ipynb                  - Script to reproduce results shown in Fig 2
├── 02_clustering_human_readable_features.ipynb     - Script to reproduce results shown in Fig 3
├── 03_clustering_transients.ipyn                   - Script to reproduce results shown in Fig 4 & 5
├── 04_kNN_predictions.ipynb                        - Script to reproduce results shown in Fig 6
└── extracted_features
    ├── test_extracted_features_and_labels.h5	    - extracted features used for testing
    ├── training_extracted_features_and_labels.h5   - extracted features used for training                    

```
The folder "extracted_features" contains the extracted features used in the paper, namely the PL transients and as well as the extracted single *in situ* feature 1 to 3 and the *ex situ* feature. The data is saved in the *.h5py format and both test and training file contain a pandas table, where each row contains a solar cell sample. 


With the following command, the packages used in the 4 notebooks can be installed from the provided requirements.txt file:

`
pip install -r requirements.txt
`

## Extracting the entire dataset 

The dataset is available on Zenodo (*add link*) as a hdf5-file and can be extracted using the notebook *00_extract_data_from_hdf5_file.ipynb*.





