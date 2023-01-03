This folder contains all data and code needed to reproduce the results of the submitted manuscript. 

For quick inspection of the generated python code, PDF print-outs of the 4 Jupyter Notebooks were added. Next to the written code, the output of the code and the generated figures, which are shown in the manuscript, can be inspected.

The *.ipynb files are Jupyter Notebooks which are interactive computational environment to execute Python code. The notebooks can be downloaded alongside the folder "extracted_features", which contains the features used in the manuscript, namely the PL transients and as well as the extracted single in situ feature 1 to 3 and the ex situ feature. The data is saved in the *.h5py format and both test and training file contain a pandas table, where each row contains a solar cell sample. 

After downloading, the notebooks can be run locally if Jupyter is setup on the local computer. For this, copy and paste the 4 notebook files, the requirements.txt, as well as the "extracted_features"-folder to the path of the local Jupyter. If unknown, the path can be found by running Jupyter, opening a new Notebook and running the command "pwd". When the files and the data have been copied to the right path, it is possible to run the files and interact with the data.

With the following command, the packages used in the 4 notebooks can be installed from the provided requirements.txt file:

pip install -r requirements.txt

If Jupyter is not installed on the local machine, the code can be run using Google colab (https://colab.research.google.com/). However, the files and the data have to be uploaded to a Google Drive. For this, create a folder "Colab Notebooks" in the Google Drive and copy and paste the 4 notebook files and the "extracted_features" folder. Rightclick one of the notebooks and choose open with "Google Colaboratory". Possibly, the app has to be added by clicking "connect more apps", then choosing the Colaboratory app and installing it. Afterwards, the code can be opened with the Colaboratory App. 
Before the code can be run, the drive has to be mounted, so that the data can be loaded from the drive. For this, add a "code"-cell (by pressing " + Code"-button), and run the following lines:

from google.colab import drive
import os
drive.mount('/content/drive')
os.chdir("/content/drive/My Drive/Colab Notebooks")

The connection to Google Drive has to be confirmed before choosing the used account and then granting colab access to the Drive.

To run notebook 4 on colab, torchmetrics has to be installed by running a cell with:

pip install torchmetrics
