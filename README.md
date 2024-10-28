**Multi-Classification of Brain Tumor Using Convolutional Neural Network**

**Project Overview**

This project focuses on the classification of brain tumors using deep learning, specifically a Convolutional Neural Network (CNN) model. The primary goal is to automate the classification of brain tumors into different glioma grades (Grade II, III, and IV) based on MRI images, thereby aiding in timely and accurate diagnosis.

**Dataset**

The model utilizes the REMBRANDT dataset, which comprises T1-weighted MRI images from The Cancer Imaging Archive (TCIA).

**The dataset includes:**

130 Patients with various glioma grades.

21223 Images of different tumor types, including Astrocytoma, Oligodendroglioma, and Glioblastoma.

**Model Architecture**

The proposed CNN model consists of:

11 Layers including convolutional, ReLU activation, max-pooling, dropout, fully connected, and softmax layers.

Activation Layers: ReLU layers follow convolutional layers to reduce vanishing gradient issues and improve feature selection.

Regularization: Dropout and L2 regularization are employed to prevent overfitting.

Optimization: The ADAM optimizer is used for efficient training.

**Key Steps**

Data Preprocessing: Images are resized to a uniform 256x256 dimension using bicubic interpolation.
Training and Validation: Data is split into training and validation sets and trained over multiple epochs.
Evaluation: Model performance is assessed using metrics derived from a confusion matrix.

**Results**

The CNN model achieved an accuracy of 87.8% for multi-class classification across three glioma grades. Performance per grade:

Grade II: 90.6%

Grade III: 88.3%

Grade IV: 84.3%

**Requirements**

Hardware: Intel i7 processor, NVIDIA GPU (GeForce MX150 or similar), 8GB RAM
Software: Python 3.7+, Pytorch, numpy, pandas, torchvision, and other libraries listed in the requirements.

**Future Work**

Future improvements include:

Expanding the dataset for enhanced accuracy.
Leveraging multiple GPUs to reduce training time.
Optimizing model architecture by increasing kernel counts and layers.
