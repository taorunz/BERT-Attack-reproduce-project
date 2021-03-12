# BERT-Attack-reproduce-project

### Intro
This repo contains code and data to reproduce the BERT-Attack paper.

The paper is: BERT-ATTACK: Adversarial Attack Against BERT Using BERT (https://arxiv.org/abs/2004.09984)

The code comes from the origin repo of the paper: https://github.com/LinyangLee/BERT-Attack


### Usage
Run the following example command to generate adversial attacks on IMDB data:

python bertattack.py --data_path data_defense/imdb.tsv --mlm_path bert-base-uncased --tgt_path target_model_path --output_dir data_defense/imdb_logs.tsv --num_label 2 --use_bpe 1 --k 48 --start 0 --end 1000 --threshold_pred_score 0

### Target Model Path
The tested model paths are listed below:

- ag: textattack/bert-base-uncased-ag-news
- imdb: textattack/bert-base-uncased-imdb
- yelp: textattack/bert-base-uncased-yelp-polarity
- fake: bert-base-uncased
