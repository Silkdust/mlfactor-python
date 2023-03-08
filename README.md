# mlfactor-python

## Introduction
This repository is some reading notes and Python implementation for book "Machine Learning for Factor Investing" by Silkdust.

For better compatibility and better accordance with original book, this repository is completed in English. 

The author of this book offers some solutions for Python Notebooks. See detailed info at https://www.mlfactor.com/python.html. However, they did not offer executable files (.ipynb). For your convenience, this project offers both jupyter notebooks (.ipynb) and a PDF version produced by `nbconvert` and XeLaTeX engine.

Finally, I deeply appreciate Guillaume Coqueret and Tony Guida for their devotions to this book. Published in 2020, this book really offers some up-to-date machine learning techniques and their applications to factor investing. They also offer a wide range of literatures in the book for interested readers. As a summary note, this project does not include all literature reviews in the book, and I encourage interested readers explore them in the [references](https://github.com/Silkdust/mlfactor-python/blob/main/REFERENCES.md) section or in the original book.

Hope you have fun reading this project!

## Depedencies
Dependencies packages will be released in the repository in future versions in `requirenments.txt`. Generally speaking, you have to install Python3 (version 3.8 or later preferred) and jupyter notebook in your device at first. To get your notebooks work properly in your device, run the following command at the beginning:
```
pip install -r requirements.txt
```

## Timelines and Contents
|  Chapter Name  | Notebook Ref | PDF Download | Status |
|  ----  | ----  | ---- | ---- |
| Chapter 1 - Notations and Data | [Here](https://github.com/Silkdust/mlfactor-python/blob/main/Chapter1-Notations.ipynb) | [Download](https://github.com/Silkdust/mlfactor-python/raw/main/notes-pdfver/Chapter1-Notations.pdf) | &#9745;Finished |
| Chapter 2 - Introduction | [Here](https://github.com/Silkdust/mlfactor-python/blob/main/Chapter2-Introduction.ipynb) | [Download](https://github.com/Silkdust/mlfactor-python/raw/main/notes-pdfver/Chapter2-Introduction.pdf) | &#9745;Finished |
| Chapter 3 - Factor Investing and Asset Pricing Anomalies | [Here](https://github.com/Silkdust/mlfactor-python/blob/main/Chapter3-Factor%20Investing%20and%20Asset%20Pricing%20Anomalies.ipynb) | [Download](https://github.com/Silkdust/mlfactor-python/raw/main/notes-pdfver/Chapter3-Factor%20Investing%20and%20Asset%20Pricing%20Anomalies.pdf) | &#9745;Finished |
| Chapter 4 - Data Preprocessing | [Here](https://github.com/Silkdust/mlfactor-python/blob/main/Chapter4-Data%20Preprocessing.ipynb) | [Download](https://github.com/Silkdust/mlfactor-python/raw/main/notes-pdfver/Chapter4-Data%20Preprocessing.pdf) | &#9745;Finished |
| Chapter 5 - Penalized Regressions and Sparse Hedging for MVP | [Here](https://github.com/Silkdust/mlfactor-python/blob/main/Chapter5-Penalized%20Regressions%20and%20Sparse%20Hedging%20for%20MVP.ipynb) |  | &#9744;Ongoing (EFT[^1]. 0309) |
| Chapter 6 - Tree-based Methods | | | &#9744;Not Started (EFT. 0312) |
| Chapter 7 - Neural Networks | | | &#9744;Not Started (EFT. 0319) |
| Chapter 8 - Support Vector Machines | | | &#9744;Not Started (EFT. 0326) |
| Chapter 9 - Bayesian Methods | | | &#9744;Not Started (EFT. 0326) |
| Chapter 10 - Validating and Tuning | | | &#9744;Not Started (EFT. 0402) |
| Chapter 11 - Validating and Tuning | | | &#9744;Not Started (EFT. 0402) |
| Chapter 12 - Portfolio Backtesting | | | &#9744;Not Started (EFT. 0409) |
| Chapter 13 - Interpretability | | | &#9744;Not Started (EFT. 0416) |
| Chapter 14 - Causality and Non-stationarity | | | &#9744;Not Started (EFT. 0423) |
| Chapter 15 - Unsupervised Learning | | | &#9744;Not Started (EFT. 0430) |
| Chapter 16 - Reinforcement Learning | | | &#9744;Not Started (EFT. 0507) |
| References | [Here](https://github.com/Silkdust/mlfactor-python/blob/main/REFERENCES.md) | [Download](https://github.com/Silkdust/mlfactor-python/raw/main/notes-pdfver/References.pdf) | &#9745;Finished |

## Acknowledgements
- Main reference: Coqueret, G., & Guida, T. (2020). *Machine Learning for Factor Investing: R Version.* Chapman and Hall/CRC.
- Other references: see [here](https://github.com/Silkdust/mlfactor-python/blob/main/REFERENCES.md). You can also find them on their website [here](https://www.mlfactor.com/solutions-to-exercises.html#ref-cao2003support).
- This project is completely **free** and uses CC0-1.0 license. We encourage reproducibility. See [here](https://github.com/Silkdust/mlfactor-python/blob/main/LICENSE) for details.

[^1]: Estimated Finished Time (before the target date in 2023).