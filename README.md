# CS6910-Assignment3
## Problem Statement
Use recurrent neural networks to build a transliteration system, using pytorch.

## Prerequisites

```
python 3.9
numpy 1.21.5
pytorch
wget
```
 - Clone/download  this repository
 - I have conducted all my experiments in Google Collab, for running in google colab, install wandb and wget(for importing dataset) using following command 
 - Enable GPU on colab for faster training
 
  ``` 
  !pip install wandb 
  !pip install wget
  ```
 - For running locally, install wandb and other required libraries using following command  
  ``` 
  pip install wandb
  pip install numpy
  pip install pytorch
  ```

## Dataset
- We use [Aksharantar dataset](https://drive.google.com/file/d/1uRKU4as2NlS9i8sdLRS1e326vQRdhvfw/view) dataset for our experiments.

# Vanilla Seq2Seq
### Hyperparameters used in experiments for Vanilla Seq2Seq
|Sr. no| Hyperparameter| Variation/values used|
|------|---------------|-----------------|
|1.| Cell type | RNN, LSTM, GRU|
|2.| Layer_size| [1,2,3,4]|
|3.| Hidden_layer_size| [64,128,256]|
|4.| Drop_out| 0,0.2,0.4,0.6 |
|5.| learning_rate| 0.001,0.0001 |


# Attention Seq2Seq
### Hyperparameters used in experiments for Attention Seq2Seq
|Sr. no| Hyperparameter| Variation/values used|
|------|---------------|-----------------|
|1.| Emb_dimension| 128,256,512|
|2.| Hidden_layer_dimension| 128,256,512|
|3.| Attn_dimension| 64,128,256|
|2.| dropout|0.3,0.5,0.6|


###  Code for Vanilla Seq2Seq and Attention Seq2Seq

The experiments for complete problem can be found [here](https://github.com/Shreyash007/CS6910-Assignment2/blob/main/Assignment2_part-A.ipynb). I have commented which part is what for better understanding


###  Excel file containing predictions against actual transliteration
- CSV file containing vanilla seq2seq predictions can be found [here](https://github.com/Shreyash007/CS6910-Assignment3/blob/main/predictions_vanilla.csv) 
- CSV file containing attention seq2seq predictions can be found [here](https://github.com/Shreyash007/CS6910-Assignment3/blob/main/predictions_attention.csv)


## Report

The wandb report for this assignment can be found [here]((https://wandb.ai/shreyashgadgil007/CS6910-Assignment3/reports/CS6910-Assignment-3--Vmlldzo0NDA5OTky)).
## Author
[Shreyash Gadgil](https://github.com/Shreyash007)
ED22S016
