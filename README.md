Random Under-Sampling:
This method randomly removes samples from the majority class to balance the class distribution. The RandomUnderSampler class from the imblearn library is used for this purpose, and the parameter sampling_strategy='majority' specifies that the majority class should be under-sampled to match the size of the minority class.

Random Over-Sampling: 
This method randomly duplicates samples from the minority class to balance the class distribution. The RandomOverSampler class from the imblearn library is used for this purpose, and the parameter sampling_strategy='minority' specifies that the minority class should be over-sampled to match the size of the majority class.

SMOTE: 
This method generates synthetic samples from the minority class by interpolating between neighboring samples. The SMOTE (Synthetic Minority Over-sampling Technique) class from the imblearn library is used for this purpose, and the parameter sampling_strategy='minority' specifies that the minority class should be over-sampled.

Tomek Links: 
This method removes samples that form "Tomek links" between the two classes, i.e., pairs of samples from different classes that are closest to each other. The TomekLinks class from the imblearn library is used for this purpose, and the parameter sampling_strategy='majority' specifies that the majority class should be down-sampled to remove Tomek links.

NearMiss: 
This method selects samples from the majority class that are closest to the minority class, based on a specified version of the NearMiss algorithm. The NearMiss class from the imblearn library is used for this purpose, and the parameter version=3 specifies the version of the NearMiss algorithm to use, while n_neighbors=3 specifies the number of nearest neighbors to consider when selecting samples.
