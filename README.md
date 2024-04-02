# Feature-Selection-and-Dimensionality-Reduction-on-California-Housing-Dataset

Explores a range of techniques aimed at enhancing predictive modeling on the California Housing dataset. This study focuses on feature selection and dimensionality reduction strategies to pinpoint crucial features and simplify dataset intricacies. By methodically evaluating methods like SelectKBest, SelectPercentile, Recursive Feature Elimination (RFE), and Principal Component Analysis (PCA), the goal is to optimize model performance and enhance interpretability for predicting house prices in California.
## Various feature selection and dimensionality reduction techniques

![feature_selection_hierarchy](https://github.com/karanshah5/Feature-Selection-and-Dimensionality-Reduction-on-California-Housing-Dataset/blob/main/images/flowchart.png)
## Implementation Details

### Dataset Details
- *Dataset:* California Housing Dataset from SKLEARN
- *Data Granularity:* Block level
- *Input:* Location, Age of house, Income, Number of rooms & bedrooms, Occupancy of household members, Population
- *Output:* House Prices
- *Source:* 1990 U.S. census
- *Number of Instances:* 20640

### Technical Details
- **Programming Language:** Python
- **Jupyter Notebook:** Google Colab
- **Packages Used:** sklearn, pandas, numpy
- **Code file:** [Feature_Selection_and_Dimensionality_Reduction_Techniques_on_California_Housing_Dataset.ipynb](https://github.com/karanshah5/Feature-Selection-and-Dimensionality-Reduction-on-California-Housing-Dataset/blob/main/Feature_Selection_and_Dimensionality_Reduction_Techniques_on_California_Housing_Dataset.ipynb)

## How to Run

The code is built on Google Colab on an iPython Notebook. 

```bash
Simply download the repository, upload the notebook and dataset on colab, and hit play!
```


## Results

| **Feature Selection Method**| R2 Score | MSE |
| -------------        | :-------------: |:------: |
| **Supervised - Filter Based Methods** |           |       |   
| Mutual Information   | 0.59   | 0.54  |
| Chi Squared   | N/A   | N/A  |
| Pearson Correlation - method 1(using f_regression and SelectKBest methods from sklearn)| 0.56 | 0.58  |
| Pearson Correlation - method 2 (using the corr() function in pandas library)   | 0.56  | .58 |
| **Supervised - Wrapper Based Methods**   |    |  |
| Recursive Feature Elimination   | 0.60   | 0.53 |
| Select From Model | N/A   | N/A  |
| Sequential Feature Selection - forward selection method  | 0.56   | 0.59  |
| Sequential Feature Selection - backward selection method  | 0.60   | 0.53  |
| **Supervised - Embedded Methods**   |    |  |
| Lasso Regularization  | 0.56   | 0.59  |
| **Random Forest**  | **0.75**   | **0.33**  |
| **UnSupervised - Dimensionality Reduction**   |    |   |
| PCA   | 0.01  | 1.31 |

**The above quant results show that we get the best result with the Random Forest from the embedded methods**

## Summary
Despite the California Housing Dataset providing a prebuilt and structured environment for experimentation, our attempts to enhance the model haven't yielded significant improvements. 

However, in real-world datasets, the crucial roles of feature selection and dimensionality reduction in improving model performance and interpretability become evident. Through systematic experimentation and evaluation of various techniques, we can identify the most suitable methods for a given dataset and modeling task, ultimately enhancing the effectiveness of predictive modeling on real-world datasets like the California Housing Dataset.
