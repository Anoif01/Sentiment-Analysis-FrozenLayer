# Sentiment-Analysis-FrozenLayer
## A study of the performance of the frozen-layer technique on the Bert model and its variants using HuggingFace's IMDB (Movie Review dataset).

Dataset link: https://huggingface.co/datasets/imdb

Finetune 5 Models: 

  -  https://huggingface.co/google-bert/bert-base-uncased
  -  https://huggingface.co/prajjwal1/bert-tiny
  -  https://huggingface.co/prajjwal1/bert-mini
  -  https://huggingface.co/prajjwal1/bert-small
  -  https://huggingface.co/distilbert/distilbert-base-uncased

###
In this study, a movie review sentiment classification task was carried out using the Huggingface official IMDB dataset.
In Bert and its variants, only the number of frozen layers, N, was studied, while other hyper-parameters were kept constant.
All experiments were conducted on Google Colab using A100 GPUs.
