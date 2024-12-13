# **XGBoost for AMES Dataset**
This project explores the application of machine learning algorithms, specifically XGBoost, for predicting the mutagenicity of chemical compounds using the AMES dataset. The primary objective is to classify compounds as mutagenic or non-mutagenic based on features derived from SMILES strings, a text-based representation of chemical structures.

## **Dataset**
The dataset used in this project is the AMES Mutagenicity dataset, accessed via the Therapeutics Data Commons (TDC) library. The dataset is automatically downloaded through the tdc library when running the code, so no manual intervention is required.
```
from tdc.single_pred import Tox
data = Tox(name = 'AMES')
split = data.get_split()
```

## **Setting Up the Virtual Environment**
This project requires Python 3.9. The code is written in Jupyter Notebook format and executed in VS Code. Anaconda is used to manage the virtual environment. Install Anaconda from https://www.anaconda.com/. Create and activate a virtual environment named ames_env and install the required dependencies as follows:
```
conda create -n ames_env python=3.9
conda activate ames_env

pip install PyTDC
pip install pandas
pip install matplotlib
pip install scikit-learn
conda install -c conda-forge rdkit
```

## **How to Run the Project**
Prepare the environment by installing the dependencies as described above. Open the final.ipynb notebook and execute the cells step by step to preprocess the data, train the model, and generate visualizations.

## Python Packages Used
This project uses the following Python packages:
- **PyTDC**: Accessing the AMES dataset.
- **pandas**: Data manipulation.
- **rdkit**: Molecular descriptor computation.
- **scikit-learn**: Model training and evaluation.
- **matplotlib**: Creating visualizations.


