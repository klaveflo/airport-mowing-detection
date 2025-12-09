# Satellite-Based Monitoring of Grassland Management: Detecting Mowing Events on Airport Areas using Machine-Learning
**Author:** Florian Klaver

## General Information
This GitHub repository contains the code for the projectwork 2 of the 5. semester in the Applied Digital Life Sciences Bachelor at ZAHW. The pipeline is split up in four seperate Jupyter Notebooks: 

- **Preprocessing.ipynb:** Preprocessing of the data, including steps such as cleaning, CRS matching etc.
- **Feature_Engineering.ipynb** Creating and engineering the Features used for model training (Vegetation Index Calculation, temporal matching of satellite images, sampling, etc.)
- **ML_Model.ipynb:** Setting up, training and evaluating different ML-Model types and configurations
- **Model_Application.ipynb:** Application of the best models on a complete scene (entire satellite images)

The data used for this project is not provided, since some of it is confidential. Nevertheless, the workflow is fully resuable with own data and can easily be adjusted for new projects thanks to the usage of modular functions and parameter definitions at the start of each notebook.

## Usage
To reuse this workflow, just clone the repository and create an environment with the requirements (environment.yml):

```bash
# Conda environment
conda env create -f environment.yml
```

Now you only need to adjust the paths and if necessary tweak some parameters to then run the pipeline on your own data. The seperate Jupyter Notebooks are meant to be run in the following order:

1. Preprocessing.ipynb
2. Feature_Engineering.ipynb
3. ML_Model.ipynb
4. Model_Application.ipynb