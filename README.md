# mlfactor-python

## Introduction
This repository is some reading notes and Python implementation for book "Machine Learning for Factor Investing" by Silkdust.

For better compatibility and better accordance with original book, this repository is completed in English. 

The author of this book offers some solutions for Python Notebooks. See detailed info at https://www.mlfactor.com/python.html. However, they did not offer executable files (.ipynb). For your convenience, this project offers both jupyter notebooks (.ipynb) and a PDF version produced by `nbconvert` and `XeLaTeX` engine.

Finally, I deeply appreciate Guillaume Coqueret and Tony Guida for their devotions to this book. Published in 2020, this book really offers some up-to-date machine learning techniques and their applications to factor investing. They also offer a wide range of literatures in the book for interested readers. As a summary note, this project does not include all literature reviews in the book, and I encourage interested readers explore them in the [references](https://github.com/Silkdust/mlfactor-python/blob/main/REFERENCES.md) section or in the original book.

Hope you have fun reading this project!

## Timelines and Contents
|  Chapter Name  | Notebook Ref | PDF Download | Status |
|  :--:  | :--:  | :--: | :--: |
| Chapter 1 - Notations and Data | [Here](https://github.com/Silkdust/mlfactor-python/blob/main/Chapter1-Notations.ipynb) | [Download](https://github.com/Silkdust/mlfactor-python/raw/main/notes-pdfver/Chapter1-Notations.pdf) | &#9745;Finished |
| Chapter 2 - Introduction | [Here](https://github.com/Silkdust/mlfactor-python/blob/main/Chapter2-Introduction.ipynb) | [Download](https://github.com/Silkdust/mlfactor-python/raw/main/notes-pdfver/Chapter2-Introduction.pdf) | &#9745;Finished |
| Chapter 3 - Factor Investing and Asset Pricing Anomalies | [Here](https://github.com/Silkdust/mlfactor-python/blob/main/Chapter3-Factor%20Investing%20and%20Asset%20Pricing%20Anomalies.ipynb) | [Download](https://github.com/Silkdust/mlfactor-python/raw/main/notes-pdfver/Chapter3-Factor%20Investing%20and%20Asset%20Pricing%20Anomalies.pdf) | &#9745;Finished |
| Chapter 4 - Data Preprocessing | [Here](https://github.com/Silkdust/mlfactor-python/blob/main/Chapter4-Data%20Preprocessing.ipynb) | [Download](https://github.com/Silkdust/mlfactor-python/raw/main/notes-pdfver/Chapter4-Data%20Preprocessing.pdf) | &#9745;Finished |
| Chapter 5 - Penalized Regressions and Sparse Hedging for MVP | [Here](https://github.com/Silkdust/mlfactor-python/blob/main/Chapter5-Penalized%20Regressions%20and%20Sparse%20Hedging%20for%20MVP.ipynb) | [Download](https://github.com/Silkdust/mlfactor-python/raw/main/notes-pdfver/Chapter5-Penalized%20Regressions%20and%20Sparse%20Hedging%20for%20MVP.pdf) | &#9745;Finished[^1] |
| Chapter 6 - Tree-based Methods | [Here](https://github.com/Silkdust/mlfactor-python/blob/main/Chapter6-Tree-based%20Methods.ipynb) | [Download](https://github.com/Silkdust/mlfactor-python/raw/main/notes-pdfver/Chapter6-Tree-based%20Methods.pdf) | &#9745;Finished |
| Chapter 7 - Neural Networks | [Here](https://github.com/Silkdust/mlfactor-python/blob/main/Chapter7-Neural-Networks.ipynb) | [Download](https://github.com/Silkdust/mlfactor-python/raw/main/notes-pdfver/Chapter7-Neural-Networks.pdf) | &#9745;Finished |
| Chapter 8 - Support Vector Machines | [Here](https://github.com/Silkdust/mlfactor-python/blob/main/Chapter8-Support-Vector-Machines.ipynb) | [Download](https://github.com/Silkdust/mlfactor-python/raw/main/notes-pdfver/Chapter8-Support-Vector-Machines.pdf) | &#9745;Finished |
| Chapter 9 - Bayesian Methods | [Here](https://github.com/Silkdust/mlfactor-python/blob/main/Chapter9-Bayesian-Methods.ipynb) | [Download](https://github.com/Silkdust/mlfactor-python/raw/main/notes-pdfver/Chapter9-Bayesian-Methods.pdf) | &#9745;Finished[^2] |
| Chapter 10 - Validating and Tuning | [Here](https://github.com/Silkdust/mlfactor-python/blob/main/Chapter10-Validating-and-Tuning.ipynb) | [Download](https://github.com/Silkdust/mlfactor-python/raw/main/notes-pdfver/Chapter10-Validating-and-Tuning.pdf) | &#9745;Finished |
| Chapter 11 - Ensemble Models | | | &#9744;Ongoing (EFT[^3]. 1028) |
| Chapter 12 - Portfolio Backtesting | | | &#9744;Not Started (EFT. 1031) |
| Chapter 13 - Interpretability | | | &#9744;Not Started (EFT. 1105) |
| Chapter 14 - Causality and Non-stationarity | | | &#9744;Not Started (EFT. 1110) |
| Chapter 15 - Unsupervised Learning | | | &#9744;Not Started (EFT. 1115) |
| Chapter 16 - Reinforcement Learning | | | &#9744;Not Started (EFT. 1120) |
| References | [Here](https://github.com/Silkdust/mlfactor-python/blob/main/REFERENCES.md) | [Download](https://github.com/Silkdust/mlfactor-python/raw/main/notes-pdfver/References.pdf) | &#9745;Finished |


## Depedencies
Dependencies packages have be released in the repository as `requirenments.txt` and will be updated regularly. Generally speaking, you have to install Python3 (version 3.8 or later preferred) and jupyter notebook in your device at first. To get your notebooks work properly in your device, run the following command after cloning this repo:
```
git clone https://github.com/Silkdust/mlfactor-python.git
cd mlfactor-python/
pip install -r ./requirements.txt
```

If you revise the coding or use additional packages, there is a **simple command** with `pipreqsnb` to remake the [`requirements.txt`](https://github.com/Silkdust/mlfactor-python/blob/main/requirements.txt) after cloning this repo as follows:
```
pip install pipreqs
pip install pipreqsnb
pipreqsnb --force ./ --encoding=utf-8
```

For better I/O speed, the `data_ml` object is stored in `.pkl` format. However, this costs a lot of storage space and is *not* pushed to the repo. You may run the following commands to generate it under the `/data/` folder:
```
import pandas as pd
import pyreadr
# data = pd.read_excel("./data/data_ml.xlsx") # Not Recommended. Too Slow!
result = pyreadr.read_r('./data/data_ml.RData')
data = result['data_ml']
data.to_pickle("./data/data_ml.pkl")
```

## Acknowledgements
- Main reference: Coqueret, G., & Guida, T. (2020). *Machine Learning for Factor Investing: R Version.* Chapman and Hall/CRC.
- Other references: see [here](https://github.com/Silkdust/mlfactor-python/blob/main/REFERENCES.md). You can also find them on their website [here](https://www.mlfactor.com/solutions-to-exercises.html#ref-cao2003support).
- This project is completely **free** and uses CC0-1.0 license. We encourage reproducibility. See [here](https://github.com/Silkdust/mlfactor-python/blob/main/LICENSE) for details.

[^1]: There are some minor differences between `ElasticNet` in `sklearn` and `glmnet` in `R`. See [here](https://stats.stackexchange.com/questions/206898/difference-between-elasticnet-in-scikit-learn-python-and-glmnet-in-r) for details.
[^2]: Two less familiarized packages in Python are faciliated in this Chapter to complete the Bayesian linear regression and the BART. For the first one, we provide the source code inside the notebook so that there is virtually no need for you to install the package `conjugate_bayes` (which is messy). 
For the second package `bartpy`, please use this command to install the `BartPy` package to avoid from the following [issues #37](https://github.com/JakeColtman/bartpy/issues/37) and [#51](https://github.com/JakeColtman/bartpy/issues/51): `pip install git+https://github.com/JakeColtman/bartpy.git@pytorch --upgrade`.
[^3]: Estimated Finished Time (before the target date in 2023). Due to the academic works and internships (and holidays) for the author, the original schedule has been postponed. The author had already re-activated the project in October.