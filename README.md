DeepAlz: Alzheimer's Disease Detection via Multiscale Feature Modelling
Welcome to DeepAlz, a research project born from a desire to tackle a critical real-world problem: the early and accurate diagnosis of Alzheimer's disease. Existing diagnostic methods can be slow and subjective. This project explores how we can build a more robust, efficient, and highly accurate detection system using modern deep learning architectures.
This is more than just a classification model. It's an end-to-end investigation into efficient network design, novel attention mechanisms, and rigorous scientific validation, culminating in a model that achieves state-of-the-art results and is published in the International Journal of Computational Intelligence Systems.
What This Project Does
🧠 High-Accuracy Diagnosis: Accurately classifies brain MRI scans into four stages of Alzheimer's, achieving 99.75% accuracy on the OASIS dataset and 96.25% on the AD-Dataset.
✨ Novel Attention Mechanism: Introduces the Improved Spatial Attention Block (I-SAB), a custom module designed to help the model focus more effectively on critical regions within MRI scans.
⚡ Computationally Efficient Design: Built on a Depth-Separable CNN backbone, making the model significantly lighter and faster than traditional CNNs without sacrificing performance.
🔬 Published, Peer-Reviewed Research: The methodology, results, and contributions of this project have been validated and published in a reputable scientific journal.
Tech Stack
This project is built in Python 3.8+ using the following core tools:
TensorFlow & Keras – For building and training the deep learning model
Scikit-learn – For performance metrics and model evaluation
Pandas – For data manipulation and management
Matplotlib & Seaborn – For data visualization and analyzing results
NumPy – For fundamental numerical operations
Features In Action: Classifying Alzheimer's Stages
The model is trained to identify and differentiate between four distinct classes from MRI scans:
Non-Demented (Healthy)
Very Mild Demented
Mild Demented
Moderate Demented
This multi-class capability is crucial for staging the disease, not just detecting its presence.
Behind the Scenes: How It Works
Efficient Backbone (Depth-Separable CNNs): Instead of using standard, computationally heavy convolutions, the model's architecture is based on depth-separable layers. This splits the convolution process into two steps (depthwise and pointwise), dramatically reducing the number of parameters and making the model faster to train.
Improved Spatial Attention (I-SAB): This is the core innovation. Unlike standard attention blocks that only use max and average pooling, the I-SAB incorporates three pooling strategies (max, average, and min). This gives the model a richer, more comprehensive understanding of the spatial features in an MRI, allowing it to better pinpoint subtle signs of disease.
Multi-Scale Feature Fusion: The I-SAB modules are plugged into multiple layers of the CNN backbone (at the 2nd, 4th, 6th, 8th, and 10th layers). This allows the model to capture disease-related features at different scales and levels of abstraction, from fine textures to broader structural changes.
Rigorous Validation: The model wasn't just trained and tested. Its performance was confirmed through extensive ablation studies (testing the model with and without key components like the I-SAB) and cross-dataset validation to ensure its results are robust and generalizable.
