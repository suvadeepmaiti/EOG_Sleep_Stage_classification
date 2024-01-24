[![License](https://img.shields.io/badge/License-Apache_2.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/ambv/black)
![GitHub pull requests](https://img.shields.io/github/issues-pr/suvadeepmaiti/EEG_Sleep_Stage_classification)
![GitHub issues](https://img.shields.io/github/issues/suvadeepmaiti/EEG_Sleep_Stage_classification)

# ENHANCING HEALTHCARE WITH EOG: A NOVEL APPROACH TO SLEEP STAGE CLASSIFICATION
This repository contains code, results, and dataset links for our ICASSP 2024 paper titled ***ENHANCING HEALTHCARE WITH EOG: A NOVEL APPROACH TO SLEEP STAGE
CLASSIFICATION***. 📝
>**Authors:** <a name="myfootnote1"><sup>1</sup></a>Shivam Kumar Sharma, <a name="myfootnote1"><sup>1</sup></a>Suvadeep Maiti, Bapi Raju

<sup>[1](#myfootnote1)</sup>Equal contribution

>**More details on the paper can be found [here](https://arxiv.org/pdf/2310.03757.pdf).**
> **Raise an issue for any query regarding the code, paper, or for any support.**

## Table of contents
- Introduction
- Highlights
- Results
- Dataset
- Getting started
- Getting the weights
- License and Citation

## Introduction 🔥

>We introduce an innovative approach to automated sleep stage classification using EOG signals, addressing the discomfort and impracticality associated with EEG data acquisition. In addition, it is important to note that this approach is untapped in the field, highlighting its potential for novel insights and contributions. Our proposed SE-Resnet-Transformer model provides an accurate classification of five distinct sleep stages from raw EOG signal. Extensive validation on publically available databases (SleepEDF-20, SleepEDF-78, and SHHS) reveals noteworthy performance, with macro-F1 scores of 74.72, 70.63, and 69.26, respectively. Our model excels in identifying REM sleep, a crucial aspect of sleep disorder investigations. We also provide insight into the internal mechanisms of our model using techniques such as 1D-GradCAM and t-SNE plots. Our method improves the accessibility of sleep stage classification while decreasing the need for EEG modalities. This development will have promising implications for healthcare and the incorporation of wearable technology into sleep studies, thereby advancing the field’s potential for enhanced diagnostics and patient comfort.

## Highlights ✨

- A supervised model trained on Electrooculogram (EOG) data beating the current SOTA models 💥.
- Complete pre-processing pipeline, augmentation, and training scripts are available for experimentation.
- Pre-trained model weights are provided for reproducibility.

## Results :man_dancing:

> Linear evaluation results on Sleep-EDF-20, Sleep-EDF-78 and SHHS datasets.

|          | Accuracy | κ | Macro F1-score |
| -------- | ------------- | ------------- | ------------- |
| Sleep-EDF-20| 79.3 | 0.72 | 74.7 |
| Sleep-EDF-153 | 73.6 | 0.68 | 70.6 |
| SHHS| 79.0 | 0.71 | 69.3 |


<!--t-SNE visualization using our method shows clear clusters and captures the sleep-staging progression observed clinically.-->

<!--<img src="/images/tsne.jpg" width="750">-->

>1D-GradCAM visualization of raw EOG epochs along with sleep micro-structures shown in green boxes.
<img src="/images/gradCAMREM.png" width="750">

>Confusion Matrics of Fold-0 on SleepEDF-20, SleepEDF-153 and SHHS datasets
<img src="/images/confusion_matrix.jpg" width="750">


## Getting started 🥷
#### Setting up the environment
COMING SOON
#### What each file does
COMING SOON
#### Training the model
COMING SOON
#### Testing the model
COMING SOON
#### Logs and checkpoints
- The logs are saved in `logs/` directory.
- The model checkpoints are saved in `checkpoints/` directory.

## Getting the weights :weight_lifting:
COMING SOON

## License and Citation 📰
Please cite the following paper if you have used this code:
```
@misc{deep2023sharma,
      title={ENHANCING HEALTHCARE WITH EOG: A NOVEL APPROACH TO SLEEP STAGE CLASSIFICATION}, 
      author={Suvadeep Maiti and Shivam Sharma and S. Mythirayee and Srijithesh Rajendran and Bapi Raju},
      year={2023},
      eprint={2310.03757},
      archivePrefix={arXiv},
      primaryClass={eess.SP}
}
