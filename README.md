
# Mortgage Approval Prediction Using Neural Networks


## Authors
### Bryce Hinkley

Github
- [@Ouroborosrex](https://www.github.com/Ouroborosrex)
Email
- bryce.hinkley @ my.utsa.com

#### Contributions

- Created model architecture
- Aquired dataset
- Created data cleaning code (encoding, regularization, choosing feautres)
- Data visualization
- Conducted experimentation (comparision of different feautres)
- Wrote research paper abstract, related works, methodology, metrics, results, future considerations, conclusion, and references
- Created slides for presentation
- Created documentation, such as comments, within code

### Alex Van Nimwegen

#### Contributions
- Created README
- Wrote introduction in research paper

## Introduction

Given the high levels of stress and uncertainty that inexperienced families often experience when applying for a mortgage loan, our team saw an opportunity to develop an app that could help make predictions that are unbiased and not influenced by any particular financial institution.
To this end, we have built a deep neural network model designed to accurately predict mortgage loan approvals. The primary objective of our project is to train this model to provide accurate and reliable predictions, without any undue influence from external factors.

While our current implementation is focused solely on building the predictive model, our ultimate goal is to develop an end-to-end application that will allow users to input their personal information and receive a prediction as to whether or not they are likely to qualify for a mortgage loan. We are committed to refining and improving our model over time, with the aim of creating a tool that is truly useful and accessible to all.

## Features

Our project incorporates multiple models to evaluate which data is most relevant for accurately predicting mortgage loan approvals. The first model incorporates both macro and micro economic data, while the second model removes much of the macroeconomic information. We are currently working on a third model that aims to remove any potential biases and provide even more accurate predictions. 

The project is written in Python and has been specifically set up to run in Google Colab. 

Our project also includes features to address common challenges in mortgage lending, such as data imbalance and irrelevant data columns. We have implemented strategies to correct for dataset imbalance and automatically remove columns that are not relevant to the project, streamlining the data preparation process and allowing for accurate model training.

## Getting Started

As the project is currently only written to be used in a python notebook, the project is intended to be opened in Google Colab and have each cell to be run from top to bottom.

In order to aquire the data, please visit consumerfinance.gov and get the hmda data found [here](https://www.consumerfinance.gov/data-research/hmda/historic-data/?geo=nationwide&records=all-records&field_descriptions=codes).

Make sure that you have the options as follows:
- Nationwide
- 2017
- All records
- HDMA codes only
So that you are able to resemble the dataset that we used. We added them to a public Google Drive and then used !gdown in our Jupyter file to aquire the data. However, feel free to have the data be aquired as you please so that you are able to add it into the DataFrame from a .csv file as shown in the code.

## Organization
Imported libraries required for the project are at the top.
Then the dataset is imported using !gdown and inserted into a pandas dataframe.
There are many cells that are just used to show what is happening to the data in each step, such as displaying columns in the data.
The data is then undersampled and split into training, testing, and validation sets.
Shuffled batches are created and layers are normalized.
After normalization, the model is created, compiled, and visualized.
Next the results of the model are displayed.
A second model is created, compiled, and its results are displayed for comparison.
A third model for removing bias data is below this but it is still being worked on.

## References

[1] Sirignano, J., Sadhwani, A., & Giesecke, K. (2016). Deep learning for mortgage risk. arXiv preprint arXiv:1607.02470.

[2] Weytjens, Hans, and Jochen De Weerdt. "Process outcome prediction: CNN vs. LSTM (with attention)." Business Process Management Workshops: BPM 2020 International Workshops, Seville, Spain, September 13–18, 2020, Revised Selected Papers 18. Springer International Publishing, 2020.

[3] Li, Meixuan, Chun Yan, and Wei Liu. "The network loan risk prediction model based on Convolutional neural network and Stacking fusion model." Applied Soft Computing 113 (2021): 107961.

[4] Kvamme, Håvard, et al. "Predicting mortgage default using convolutional neural networks." Expert Systems with Applications 102 (2018): 207-217.

[5] “Download HMDA data | Consumer Financial Protection Bureau,” Consumer Financial Protection Bureau. https://www.consumerfinance.gov/data-research/hmda/historic-data/

