# Evaluation

### Why is this done?

Evaluation of segmentation results ensures the accuracy and reliability of the algorithms, directly impacting clinical decisions. Researchers can validate the performance of their algorithms, identify areas for improvement, and compare different methods to select the most effective one. This helps in achieving high precision and reproducibility, ultimately leading to better patient outcomes and advancements in medical research. Accurate segmentation is essential for diagnosing diseases, planning treatments, and monitoring disease progression.&#x20;

### How is it done?

Some common methods for evaluating segmentation in MIA include:

* **Dice Similarity Coefficient (DSC)**: Measures the overlap between the predicted segmentation and the ground truth.
* **Jaccard Index**: Similar to DSC, it evaluates the intersection over union of the predicted and true segmentations.
* **Sensitivity (Recall)**: Assesses the proportion of actual positives correctly identified by the segmentation.
* **Specificity**: Evaluates the proportion of actual negatives correctly identified.
* **Precision**: Measures the proportion of predicted positives that are true positives.
* **Hausdorff Distance**: Calculates the maximum distance between the boundary points of the predicted and true segmentations.
* **Cohen’s Kappa**: Assesses the agreement between the predicted segmentation and the ground truth, accounting for chance agreement.
* **ROC Curves and AUC**: Used to evaluate the performance of binary classifiers, plotting true positive rate against false positive rate.

### Project ideas

Which metrics are suitable for our task beyond dice coefficient? What is the influence of the specific validation procedure on the results - can we under/over estimate performance if done wrongly?

* Metric types - overlap based, distance based?
* Influence of e.g. small structures - thalamus versus white-matter?
* Influence of validation procedure - using stratified subsets for fine-grained evaluations.

### Coding Resources

See `pymia.evaluation` package

### References

A. A. Taha and A. Hanbury, Metrics for evaluating 3D medical image segmentation: analysis, selection, and tool, BMC Med. Imaging, vol. 15, no. 1, pp. 1–28, 2015.

[Cross-validation](https://medium.com/towards-data-science/cross-validation-in-machine-learning-72924a69872f) in machine learning
