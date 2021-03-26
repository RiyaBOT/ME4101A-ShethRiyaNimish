# ME4101A-ShethRiyaNimish
# Final Year Project


The package implements three different techniques to classify two dimensional materials into ferromagnetic materials, anti-ferromagnetic materials and non-magnetic materials. 

The three techniques are:

- Classical Machine Learning.
- Deep Learning.
- Graph Networks.


## Table of Contents

- [Prerequisites](#prerequisites)
- [Usage](#usage)
  - [Data Featurizing](#define-a-customized-dataset)
  - [Classical Machine Learning](#train-a-cgcnn-model)
  - [Deep Learning](#predict-material-properties-with-a-pre-trained-cgcnn-model)
  - [MEGNET](#megnet)
  - [CGCNN](#cgcnn)
- [Web Interface](#wi)
- [Files](#files)
- [Authors](#authors)




##  Prerequisites

This package requires:

- [PyTorch](http://pytorch.org)
- [scikit-learn](http://scikit-learn.org/stable/)
- [pymatgen](http://pymatgen.org)
- [keras](https://keras.io)
- [matminer](https://matminer.readthedocs.io/en/latest/)


If you are new to Python, the easiest way of installing the prerequisites is via [conda](https://conda.io/docs/index.html). Other minor requirements are mentioned in the requirements.txt document



## Usage

### Data Featurizing
The code that was used for data featurizing is used in Jupyter Notebook Python. The Jupyter Notebook was preferred to a general Python script because it could be executed in a chunk wise manner and user friendly manner.
To use the same code as used in this report, it should be ensured that data is either in the format of a .csv or a .json and it is in the same folder as the Jupyter Notebook. Enter the file name and type of the file in the notebook, and enter a few other input parameters while running the Jupyter Notebook such as whether imputation needs to be performed or not and if the number of data needs to be reduced and if yes, by how much.
After the Jupyter Notebook is executed, a document DFDP-Results.docx will be saved in the same folder which will give an in-depth analysis of everything that took place during the processes of data featurizing and data-preprocessing. Furthermore, there will be another document DataAfterDFDP.csv which will store the prepared data that can then be used for machine learning and deep learning algorithms. The code here belongs to Sheth Riya Nimish.

### Classical Machine Learning
The code that was used for machine learning is used in Jupyter Notebook Python. Ensure your data is in the .csv format. The last column of your data should be the target feature. Once the machine learning algorithm is executed a document MachineLearning.docx will be saved and a model.pkl will be saved as well. Model.pkl is the best model obtained after trying out different algorithms and optimising parameters and the document gives a glimpse of every single result obtained for each algorithm and every instance in the optimisation process. The code here belongs to Sheth Riya Nimish.

### Deep Learning
The code that was used for deep learning is used in Jupyter Notebook Python. Ensure your data is in the .csv format. The last column of your data should be the target feature. The deep learning code has two different models, functional and sequential. The best model obtained after the optimisation by the author has already been hard-coded in one of the sections for use. It is also possible to do the optimisation process all over again but do note that it is computationally heavy and time-intensive. Once the deep learning algorithm is executed a document DeepLearning.docx will be saved. The document gives a glimpse of every single result obtained for each of the models. The code here belongs to the Sheth Riya Nimish.

### CGCNN
Here, only the optimisation process was done by the author. The model does not belong to the author. The original model github can be found here with the detailed instructiond for usage: [cgcnn](https://github.com/txie-93/cgcnn/tree/master/data).


### MEGNET
Here, only the optimisation process was done by the author. The model does not belong to the author. The original model github can be found here with the detailed instructiond for usage: [megnet](https://github.com/materialsvirtuallab/megnet).

## Web Interface
The best model that was obtained by the author can be found here:
- [Model to classify into Magnetic and Non Magnetic Materials](https://github.com/RiyaBOT/ME4101A-ShethRiyaNimish/blob/master/WebInterface/model.pkl)
- [Model to classify into Ferromagnetic and Anti-Ferromagnetuc Materials](https://github.com/RiyaBOT/ME4101A-ShethRiyaNimish/blob/master/WebInterface/model2.pkl)

However, it is much easier to use the web interface created by the author for the prediction of the magnetic orientation, which can be found here:
- [Web Interface](https://twodferromagnetism-model.herokuapp.com)
## Files
- Data Preparation.ipynb:  Jupyter Notebook used for data preparation
- Machine Learning.ipynb:  Jupyter Notebook used for conducting classical ma-chine learning
- Deep  Learning.ipynb:  Jupyter  Notebook  used  for  conducting  deep  learningalgorithms.
- CGCNN
 <br />CIF Data 
   – Crystal Graph Convolutional Nueral Netwroks.ipynb:  Jupyter notebookfor optimising and predicting the accuracy of CGCNN
   – Miscellaneous files such as the model, predict.py written by [21].
- Web Interface
 – model.pkl: Best model obtained during training to classify materials intomagnetic and non-magnetic.
 – model2.pkl:  Best  model  obtained  during  training  to  classify  magneticmaterials into ferromagnetic and anti-ferromagnetic materials.
 – averages.csv:  Stores the average value of the data stored.
 – data.csv:  The data used for training the above models
 – app.py:  The python file which helps in reading the input from the file.
 – index.html:  Stores the format of the app
 – mlmodel.py:  Helps in the facilitation of app.py
 – static:  Contains the fonts used in the web interface
- Documents
 – DFDP2DMatpedia.docx: Document containing results after data featurizing on 2DMatpedia.
 – DFDPC2DB.docx:  Document  containing  results  after  data  featurizingon C2DB.
 – ML.docx: Example Document containing results after Machine Learning.
 – DL.docx:  Example Document containing results after Deep Learning.
- Pictures:  Contains various graphics which are used in the jupyter notebooks
- Requirements  Text:  The  python  libraries  which  are  needed  to  execute  mycode.
- Data:
- Miscellaneous Data:  Data(NM/M)for ML, DL
 – CIF Data for CGCNN
 – DatawithFM/AFMClassification.csv
 – Data.json json file obtained from 2Dmatpdia
 – c2db.db a database obtained from computational 2d materials databse
- Surface Plots:  Matlab Code
- MEGNET
 – Graph Network.ipynb: Jupyter notebook to compute the accuracy of the MEGNET model.
## Authors

The code was primarily written by Sheth Riya Nimish who was advised by Prof. Shen Lei. 
Appropriate citations can be found in the code itself for borrowed code.

