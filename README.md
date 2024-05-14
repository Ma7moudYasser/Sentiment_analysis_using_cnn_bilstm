## Sentiment Analysis of User-Generated Data Using CNN-BiLSTM Model

This repository contains the code for the sentiment analysis model described in the research paper:

> **Abstract:** With the availability of user-generated data, like reviews, it has become possible to gain valuable information that can help service providers improve their services. Sentiment analysis is a popular method used to extract information from these reviews, but it can be challenging due to irregularities and ambiguities in the data. This chapter proposes a novel model architecture that enhances sentiment analysis and provides more accurate results than state-of-the-art technology. [...]

**Keywords:** Convolutional Neural Network · Bidirectional-Long short term memory · Sentiment Analysis

### Dataset

The model is trained on two datasets:

* **Airline-quality sentiment dataset**: This dataset contains reviews of various British airlines collected from skytrax.com. It can be accessed from Kaggle [https://www.kaggle.com/datasets/crowdflower/twitter-airline-sentiment](https://www.kaggle.com/datasets/crowdflower/twitter-airline-sentiment). The dataset is balanced with approximately equal positive and negative reviews.
* **Twitter Airline dataset**: This dataset contains tweets about US airlines and their sentiment labels (positive or negative). It was obtained from CrowdFlower's library.

### Model Architecture

The proposed model is a hybrid architecture that combines a Convolutional Neural Network (CNN) with a Bidirectional Long Short-Term Memory (BiLSTM) network. This architecture helps capture both local features and long-range dependencies in the text data.

### Evaluation

The model's performance is evaluated using several metrics:

* Accuracy
* Precision
* Recall
* F1 score

The equations for these metrics are provided in the research paper.

### Getting Started

This repository includes the following files:

* `model.py`: Contains the implementation of the CNN-BiLSTM model.
* `train.py`: Script for training the model.
* `evaluate.py`: Script for evaluating the model on a test set.
* `data_preprocessing.py`: Script for preprocessing the text data.
* `requirements.txt`: Text file containing the required Python libraries.

**Prerequisites:**

* Python 3.6 or later
* TensorFlow v2.0

**Instructions:**

1. Clone this repository.
2. Install the required libraries: `pip install -r requirements.txt`
3. Download the datasets and place them in a designated folder.
4. Modify the data paths in the relevant scripts (`data_preprocessing.py`, `train.py`, `evaluate.py`) to point to your downloaded datasets.
5. Run the training script: `python train.py`
6. Evaluate the trained model: `python evaluate.py`

### Citation

If you use this code in your research, please cite the following paper:

```bibtex
@InProceedings{rao2023sentiment,
  title={Sentiment Analysis of User-Generated Data Using CNN-BiLSTM Model},
  author={Rao, M. and Shaw, R. N. and et al.},
  booktitle={ICACIS 2023},
  editor={Shaw, R. N. and et al.},
  volume={1920},
  pages={239--246},
  series={CCIS},
  year={2023},
  publisher={Springer Nature Switzerland AG},
  doi={10.1007/978-3-031-45121-8_20}
}
