# hong-kong-fastText
fastText vectors created from Hong Kong data.

## Corpus
* ToastyNews crawled Hong Kong news websites (private data) (late 2015 - March 2019)
* Yue Wikipedia (March 2019)
* The Encyclopedia of Virtual Communities in Hong Kong (April 2017)

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

## Vectors
* bin https://storage.googleapis.com/com_toastynews_public/toastynews.bin.gz
* txt https://storage.googleapis.com/com_toastynews_public/toastynews.vec.gz
