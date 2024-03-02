# Sentiment-Analysis-FrozenLayer
## A study of the performance of the frozen-layer technique on the Bert model and its variants using HuggingFace's IMDB (Movie Review dataset).

## Introduction
**Does fine-tuning the whole model always yield the best results ?**
In this study, I use the Huggingface IMDB dataset for a sentiment classification task of movie reviews. While keeping other hyperparameters constant, I vary the number of frozen layers (N) in Bert and its variants. The experiments were all conducted on Google Colab, using A100 GPUs.

## Some conclusions
**Model Optimization Insights**
This recent analysis provides valuable insights into enhancing model performance effectively. The findings indicate that **optimal results are achieved by freezing approximately half of the encoder layers** (e.g., N=2, 4, 6). This strategy highlights that **the initial layers of pretrained models possess universally applicable knowledge crucial** for various NLP tasks, which should be preserved during the fine-tuning process to mitigate over-fitting risks.

Furthermore, the freeze-layer technique not only boosts model accuracy but also considerably reduces training time. This approach facilitates an efficient and effective equilibrium between performance improvement and computational efficiency.

_Note: These observations are derived from a sentiment classification task and may vary across different NLP applications._


## References
Dataset: 

  - https://huggingface.co/datasets/imdb

Finetune 5 Models: 

  -  https://huggingface.co/google-bert/bert-base-uncased
  -  https://huggingface.co/prajjwal1/bert-tiny
  -  https://huggingface.co/prajjwal1/bert-mini
  -  https://huggingface.co/prajjwal1/bert-small
  -  https://huggingface.co/distilbert/distilbert-base-uncased



