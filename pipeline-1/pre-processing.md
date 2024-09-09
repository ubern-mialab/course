# Pre-processing

### Why is this done?

Preprocessing aims to enhance the quality of the images and prepare them for further analysis. In this section, we investigate the influence of pre-processing on the segmentation performance.

Common preprocessing steps include:

* **Noise Reduction**: Removing unwanted noise using filters like Gaussian or median filters.
* **Normalization**: Adjusting the intensity values to a standard range.
* **Resampling**: Adjusting the image resolution to ensure consistency across different images.
* **Segmentation**: Isolating regions of interest (e.g., organs, tumors) from the background.

### How is it done?

Some well understood algorithms in this step include:&#x20;

* Histogram matching
* Skull stripping (separate the brain from the skull and other surrounding structures)

###

### Coding Resources

* `pymia.filtering.preprocessing`
* `medpy.filter.IntensityRangeStandardization.IntensityRangeStandardization <http://loli.github.io/medpy/generated/medpy.filter.IntensityRangeStandardization.IntensityRangeStandardization.html#medpy.filter.IntensityRangeStandardization.IntensityRangeStandardization>`\_



TODO: also list project ideas in this component.

### References

L. G. Nyúl, J. K. Udupa, and X. Zhang, New variants of a method of MRI scale standardization, IEEE Trans. Med. Imaging, vol. 19, no. 2, pp. 143–50, Feb. 2000.

J.-P. Bergeest and F. Jäger, A Comparison of Five Methods for Signal Intensity Standardization in MRI, in Bildverarbeitung für die Medizin 2008, Berlin Heidelberg: Springer, 2008, pp. 36–40.

scikit-learn: Pre-processing data \<http://scikit-learn.org/stable/modules/preprocessing.html#preprocessing>\_
