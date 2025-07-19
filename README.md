DeepAlz: Alzheimer's Disease Detection via Multiscale Feature Modelling

Our model introduces a novel, computationally efficient deep learning architecture for the multi-class classification of Alzheimer's disease stages from MRI scans, achieving state-of-the-art performance on benchmark datasets.

**Key Features & Achievements:** 
    State-of-the-Art Performance: Achieved an accuracy of 99.75% on the OASIS dataset and 96.25% on the Kaggle AD dataset, outperforming previous models.
    Novel Architecture: Built on a lightweight 10-layer depth-separable CNN, making it faster and more efficient than standard CNNs.
    Improved Spatial Attention (I-SAB): Developed a novel attention mechanism that enhances the model's ability to focus on critical regions within MRI scans by using max, average, and min pooling strategies.
    Robust & Validated: The model's effectiveness was rigorously tested through extensive experiments, including 6 ablation studies and a domain generalization test on over 6,000 MRI scans.
    Results
    Our model demonstrates a significant improvement over existing methods on two publicly available datasets.
    Performance on Kaggle AD Dataset
    Model	Accuracy (%)	Precision (%)	Recall (%)	F1-Score (%)
    Inception-V4	73.75	-	-	45.05
    DEMNET	85.00	80.00	88.00	83.00
    ADDTLA	91.70	91.50	93.70	92.50
    Proposed Model (Ours)	96.25	96.71	96.36	96.52
    Performance on OASIS Dataset
    Model	Accuracy (%)	Precision (%)	Recall (%)	F1-Score (%)
    Ensamble-hybrid deep net	95.23	-	-	-
    DeepNet	99.68	-	-	99.99
    Proposed Model (Ours)	99.75	99.63	99.91	99.77
💾 Datasets
This project utilizes two publicly accessible datasets. Please download them from their original sources:
Alzheimer's Dataset (4 class of images): Available on Kaggle. This dataset contains MRI scans categorized into four stages: Mild Demented, Moderate Demented, Non-Demented, and Very Mild Demented.
OASIS-1: The Open Access Series of Imaging Studies (OASIS) is available at OASIS Brains.
You will need to preprocess and structure these datasets as expected by the data loader scripts.




