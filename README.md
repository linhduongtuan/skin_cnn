# skin_cnn
## Basic Framework for CNN-based Image Classification of ISIC 2019 Dataset

#### Here you can find two notebooks that go over basic implementation of image classification using convolutional neural networks (CNN) in Pytorch.

Data loading and augmentation is covered in the [dataprep](https://github.com/robinfchan/skin_cnn/blob/master/dataprep.ipynb) notebook.

CNN training (using transfer learning) and evaluation is covered in the [cnn_training_and_eval](https://github.com/robinfchan/skin_cnn/blob/master/cnn_training_and_eval.ipynb) notebook.

## Requirements
#### Data
For these examples I'm using the ISIC 2019 dataset from: [https://challenge2019.isic-archive.com/](https://challenge2019.isic-archive.com/)
\nThis is a publicly available curated set of >25K annotated images for eight different classes of skin lesions.

#### Packages
python | pytorch | torchvision | scikit-learn | tqdm

Dependancies:
  * scipy
  * numpy
  * pandas
  * matplotlib
  * pillow (see below)

Conflicts:\npytorch v1.4 and lower & pillow v7+ don't play nice together -- either use the pytorch nightlies (1.5 or higher) or force install pillow==6
  
Runtimes:\nCUDA -- it's strongly recommended that training be done on GPU, otherwise it is S L O W
