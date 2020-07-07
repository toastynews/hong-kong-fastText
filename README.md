# hong-kong-fastText
*Updated July 2020* 

fastText vectors created from Hong Kong data.

## Corpus
* ToastyNews crawled Hong Kong news websites (private data) (late 2015 - May 2020)
* Yue Wikipedia (May 2020)
* The Encyclopedia of Virtual Communities in Hong Kong (May 2020)
* Forums
* Restaurant Reviews
* Internet Fiction

## Preprocessing
1. Cleaned up tags from the Wikipedia/Wikia dumps.
2. Segmentation by Jieba with a custom ToastyNews dictionary.

## Parameters
These should be similar to the official vectors.
cbow
-minn 2 
-dim 300 
-epoch 10 
-neg 10
-minCount 20

## Evaluation

These vectors (HK) are compared to the [Facebook pre-trained word vectors for 157 languages](https://fasttext.cc/docs/en/crawl-vectors.html)

|Benchmark        |Facebook |HK     |
|-----------------|--------:|------:|
|Dimensions       | 300     | 300   |
|Vocab Size       |2,000,001|222,907|
|Tokens           |30,176M  |246M   |
|Analogy - Capital| 0.43    |  0.53 |
|Analogy - City   | 0.59    |  0.08 |
|Analogy - Family | 0.58    |  0.52 |
|WS-240           | 0.48    |  0.54 |
|WS-297           | 0.59    |  0.62 |
|SimLex-999       | 0.35    |  0.40 |

## Vectors
* [toastynews.vec.gz](https://drive.google.com/file/d/1NOkKfGMQPg7QfqNNj2Y46Xr4YbCbQZcZ/view?usp=sharing) - standard format
* [toastynews.bin.gz](https://drive.google.com/file/d/1kmZ8NKYDngKtA_-1f3ZdmbLV0CDBy1xA/view?usp=sharing) - if advanced functionality is needed
