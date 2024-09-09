# Feature Extraction

### Why is this done?

Feature extraction in medical image analysis is crucial for transforming raw image data into meaningful information that can be used for diagnosis, classification, and prediction. By identifying and isolating relevant features, enhancing the accuracy and efficiency of subsequent tasks. These features can be:

* **Shape Features**: Describing the geometry of structures (e.g., area, perimeter, compactness).
* **Texture Features**: Analyzing the texture patterns within the image (e.g., contrast, entropy).
* **Intensity Features**: Measuring the intensity values within regions of interest.

### How is it done?

Feature extraction in medical image analysis involves several key steps and techniques. Here are some well researched methods:

* **Local Binary Patterns (LBP)**: Captures texture features by comparing pixel intensities.
* **Gray-Level Co-occurrence Matrix (GLCM)**: Analyzes spatial relationships between pixels to extract texture features.
* **Gray-Level Run-Length Matrix (GLRM)**: Measures the length of consecutive pixels with the same intensity.
* **Completed Local Binary Patterns (CLBP)**: An extension of LBP that includes additional information about pixel intensity variations.
* **Feature Fusion**: Combining multiple features to improve the accuracy and robustness of the analysis.
* **Deep Learning Approaches**: Utilizes neural networks to automatically learn and extract features from images.

### Project ideas

A typical optimization for faster processing is to check if we can reduce the number of features to decrease the model complexity and the computational burden. Some steps in this direction could include:

* Decision forest feature importance
* Principal component analysis (PCA)
* Mutual information based feature selection

Furthermore, what features could be used to improve our model?

* Investigate other features
  * Hemisphere feature
  * Filter banks
  * Histogram of oriented gradients (HOGs)
* 2-D / 3-D differences

### Coding Resources

[scikit-image](https://scikit-image.org/docs/dev/api/skimage.feature.html): feature module

[scikit-learn](http://scikit-learn.org/stable/modules/decomposition.html#decompositions): Dimensionality reduction

[Parallelized Mutual Information](https://github.com/danielhomola/mifs) based Feature Selection

### References

H. Peng, F. Long, and C. Ding, Feature selection based on mutual information criteria of max-dependency, max-relevance, and min-redundancy, IEEE Transactions on Pattern Analysis and Machine Intelligence, vol. 27, no. 8, pp. 1226-38, 2005.
