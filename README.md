# Aggregation Tool for Genomic Concepts (ATGC)
ATGC is a deep learning model for featurizing instance level data and performing classification or regression tasks at the sample level with multiple instance learning.  For example, the model could be used to classify tumor type based on features extracted from instances such as somatic mutations.  In addition to instance features, the model also allows for sample features to be included.  Built with Python 3 and TensorFlow 2 and tf.keras, the scripts have been tested on TF 2.1, and 2.2.

The fastest way to get started would be to create some simulated data with https://github.com/OmnesRes/ATGC/blob/master/figures/controls/samples/sim_data.py, and then run a classification task on that data with https://github.com/OmnesRes/ATGC/blob/master/figures/controls/samples/sim_run.py.

The model was developed for somatic mutation data and the currently available featurization classes are for this data type (VariantSequence and VariantPositionBin in CustomKerasModels.py).  To apply the model to another data type all a user would have to do is add their own featurization class.

## Publication
The code for this repository accompanies the following paper: https://www.biorxiv.org/content/10.1101/2020.08.05.237206v1.  Files which were small enough to upload or which aren't publically available have been included.  Larger files will have to be downloaded from the links provided as comments in the Python scripts.
