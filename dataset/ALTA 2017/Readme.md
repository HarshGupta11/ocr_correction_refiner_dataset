# ALTA 2017 Challenge

These files were used in the [ALTA 2017 Challenge](http://www.alta.asn.au/events/sharedtask2017/index.html). The competition was hosted by [Kaggle in Class](https://www.kaggle.com/c/alta-2017-challenge).

If you use these data, please cite:

D. Mollá, S. Cassidy. Overview of the 2017 ALTA Shared Task:
Correcting OCR Errors (2017). *Proc. ALTA 2017*.
[https://aclanthology.coli.uni-saarland.de/papers/U17-1014/u17-1014](https://aclanthology.coli.uni-saarland.de/papers/U17-1014/u17-1014)


## File descriptions

*    `convert.py` - python script for converting files
*    `train_input.csv` - the training set
*    `train_output.csv` - the training set with all OCR errors corrected
*    `train_output_bigrams.csv` - the solutions of the training set. This file is the actual output of the conversion script using the file train_output.csv as input.
*    `test_input.csv` - the test set
*    `test_baseline_bigrams.csv` - a sample submission file in the correct format. This file contains the set of bigrams found in test_input.csv, and the resulting F1 score is zero (or close to zero according to the evaluation performed by Kaggle in Class).
