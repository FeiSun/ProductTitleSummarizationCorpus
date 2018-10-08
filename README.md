# Product Title Summarization(PTS) Corpus

 

Dataset for CIKM 2018 paper "Multi-Source Pointer Network for Product Title Summarization"

### Description 

Each line in corpus.txt consists of a pair of titles (original title, short title),  their brands, and commodity names. Each line is `tab-delimited` (two tabs) with the following format:

```bash
<original title>\t\t<short title>\t\t<brand>\t\t<commodity name>
```

#### File

* **corpus**: the dataset used in the cikm 2018 paper, the length of short title < 11.

* **big_corpus**: much larger dataset,  the length of short title < 13.

  We split the file into 5 files with prefix `big_corpus.tar.gz_` due to the limitation on github.com (less than 100m). 

  The way to reconstruct the big_corpus file:

  ```bash
  cd big_corpus
  cat big_corpus.tar.gz_* > big_corpus.tar.gz
  tar zxvf big_corpus.tar.gz
  ```

  



**Note:**

`brand` may contain multi-language versions(separated using “/”) for some products, e.g., Nintendo/任天堂. 



### Citation

```
@inproceedings{Sun:CIKM2018,
author = {Fei Sun and Peng Jiang and Hanxiao Sun and Changhua Pei and Wenwu Ou and Xiaobo Wang},
title = {{Multi-Source Pointer Network for Product Title Summarization}},
booktitle = {CIKM},
year = 2018
}
```

