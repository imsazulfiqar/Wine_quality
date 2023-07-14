# Wine_quality

Link to dataset: https://archive.ics.uci.edu/ml/machine-learning-databases/wine-quality/

#Initial Analysis and Work Done on Dataset:

The dataset from UCI is divided into red and white wine dataset, white wine dataset was used as it had more instances than the
red wine dataset, it contained 4898 instances. It has 11 feature columns and 1 target multi-class column of wine quality ranging
from the values 3-9, 3 being poor and 9 being excellent wine quality. The dataset does not contain any missing or null values and
the distribution of the target class is heavily imbalanced where classes 5 and 6 heavily outnumbered the other classes, making up
75% of the population. The outliers in the dataset were removed using Interquartile range. The early versions of the model we
trained on this dataset had a maximum accuracy of 55-60%, this may be due to the complex and imbalanced nature of the dataset.
This problem was solved by feature engineering, as the dataset was split into 2 groups of qualities 3-5 which was labelled as 0
and 6-9 labelled as 1, making the work a binary classification task. Furthermore, the training features were normalised before
being fed to the neural network. This improved the accuracy of the model and brought it to the range of 75-80%. The dataset was
used in Cortez et al (2009), with NECO methods such as multi-layer perceptrons and support-vector machines (SVMs) being
applied to it. In that paper, SVMs performed the best, although it was used for a regression task. This dataset was also used in Di
(2022), where they rearranged the features using PCA and applied 1D-CNN and further optimised the features using
backpropagation. In this paper, they also compared the performance of CNN to other methods and CNN gave the best accuracy of
83%.
