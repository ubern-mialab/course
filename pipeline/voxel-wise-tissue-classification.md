# Voxel-wise tissue Classification

### Why is this done?

Classification assigns labels to different regions or structures within the image based on the extracted features. It allows for the precise identification and isolation of specific regions of interest within an image, such as organs, tissues, or abnormalities. This process enhances the accuracy of diagnosis and treatment planning by providing detailed information about the shape, size, and location of these regions.

### How is it done?

This step often involves machine learning algorithms such as:

*   **Random Forest (**<mark style="color:blue;">**what we will use as the default implementation**</mark>**)**:

    An ensemble method that uses multiple decision trees, reduces overfitting by averaging multiple trees, while providing feature importance scores for interpretability.
*   **Support Vector Machines (SVM)**:

    Effective for high-dimensional spaces, uses a hyperplane to separate different classes, and can be used for both classification and regression tasks.
*   **XGBoost (Extreme Gradient Boosting)**:

    An efficient and scalable implementation of gradient boosting, combining the predictions of multiple weak learners to improve accuracy. Important to include regularization techniques to prevent overfitting.
*   **K-Nearest Neighbors (KNN)**:

    Classifies based on the majority class among the k-nearest neighbors. This is simple and intuitive, but can be computationally expensive for large datasets.
*   **Naive Bayes**:

    Based on Bayes’ theorem with the assumption of independence between features. It works well with small datasets and is easy to implement.&#x20;
*   **Logistic Regression**:

    A statistical model that uses a logistic function to model binary outcomes. It provides probabilities for class membership, and is simple and interpretable.
* **Deep Learning Models**: This class of algorithms includes Convolutional Neural Networks (CNNs) for more complex and accurate tasks.

### Project ideas

Do other machine learning algorithms perform better on our task? Can we improve the segmentation performance by parameter tuning?

* Overfitting
* Parameter tuning (tree depth, forest size)
* Support Vector Machine (SVM)
* Variants of decision forests (e.g., gradient boosted trees)

### Coding Resources

[scikit-learn](http://scikit-learn.org/stable/supervised\_learning.html#supervised-learning): Supervised learning

[Generic U-Net](https://github.com/jakeret/tf\_unet) Tensorflow implementation for image segmentation

[U-Net PyTorch](https://pytorch.org/hub/mateuszbuda\_brain-segmentation-pytorch\_unet) implementation for brain MRI

### References

A. Criminisi and J. Shotton, Decision Forests for Computer Vision and Medical Image Analysis, 1st ed. London: Springer, 2013.

R. S. Olson, W. La Cava, Z. Mustahsan, A. Varik, and J. H. Moore, Data-driven Advice for Applying Machine Learning to Bioinformatics Problems, Aug. 2017.

O. Ronneberger, P. Fischer, and T. Brox, U-Net: Convolutional Networks for Biomedical Image Segmentation, May 2015.
