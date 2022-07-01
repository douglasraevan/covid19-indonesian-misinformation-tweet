# COVID-19 Indonesian Misinformation Tweets

This is a repository to store an annotated dataset for COVID-19 Indonesian Misinformation Tweets. The tweet collection ranges from January 27, 2020 until February 7, 2021. 

## Paper

This repository is a byproduct of our research in which the preprint can be accessed on https://arxiv.org/abs/2206.15359. Please cite this paper accordingly if you plan to use this dataset for your publications.

## Data Collection

The original tweet data were collected through two methods:
- *In-house data collection*: Data were gathered by scraping directly from Twitter API (Original dataset repo: https://github.com/douglasraevan/covid19-indonesian-tweet)
- *Secondary data*: Additional data were retrieved from https://github.com/thepanacealab/covid19_twitter to cover the missing data collection period prior to July 21, 2020.

## Annotation

Several non-expert annotators were employed to annotate each tweet. After resolving the annotations from different annotators, there are six different labels found:
- `true`
- `misinformation`
- `irrelevant`
- `no_consensus`
- `not_sure`
- `need_expert_judgment`

## How to Use

Following Twitter API's developer policy, we only publish the tweet ID and its annotated label. *Hydrating* the tweet ID with the full data can be done by using available tools such as DocNow's hydrator (https://github.com/DocNow/hydrator) or by directly retrieving the data from Twitter API.

| id           | label     |
|--------------|-----------|
| <tweet_id_1> | <label_1> |
| <tweet_id_2> | <label_2> |
| ...          | ...       |
| <tweet_id_N> | <label_N> |

## How to Cite

### Bibtex

```
@misc{faisal2022twostage,
      title={Two-Stage Classifier for COVID-19 Misinformation Detection Using BERT: a Study on Indonesian Tweets}, 
      author={Douglas Raevan Faisal and Rahmad Mahendra},
      year={2022},
      eprint={2206.15359},
      archivePrefix={arXiv},
      primaryClass={cs.CL}
}
```



