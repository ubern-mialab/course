# Feature Extraction

### Why is this done?

Feature extraction involves identifying and quantifying specific characteristics within the image. These features can be:

* **Shape Features**: Describing the geometry of structures (e.g., area, perimeter, compactness).
* **Texture Features**: Analyzing the texture patterns within the image (e.g., contrast, entropy).
* **Intensity Features**: Measuring the intensity values within regions of interest.

### How is it done?

Can we reduce the number of features to decrease the model complexity and the computational burden.

* Decision forest feature importance
* Principal component analysis (PCA)
* Mutual information based feature selection

What features could be used to improve our model?

* Investigate other features
  * Hemisphere feature
  * Filter banks
  * Histogram of oriented gradients (HOGs)
* 2-D / 3-D differences

### Coding Resources

`scikit-image feature module <http://scikit-image.org/docs/dev/api/skimage.feature.html>`\_

`scikit-learn: Dimensionality reduction <http://scikit-learn.org/stable/modules/decomposition.html#decompositions>`\_

`Parallelized Mutual Information based Feature Selection <https://github.com/danielhomola/mifs>`\_

TODO: also list project ideas in this component.

### References

H. Peng, F. Long, and C. Ding, Feature selection based on mutual information criteria of max-dependency, max-relevance, and min-redundancy, IEEE Transactions on Pattern Analysis and Machine Intelligence, vol. 27, no. 8, pp. 1226-38, 2005.
