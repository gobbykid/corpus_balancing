## Balancing the corpus: criteria 

Given our research questions, we want our female and male corpora to be *large enough*, in order to allow meaningful results, while at the same time being *balanced* according to certain criteria, in order for our dataset to be represenative of the whole population we are considering. 

The process presented in this notebook is aimed at filtering the works in the original dataset in order to get two corpora satisfying the following criteria:
1. **Largest possible dimension**: we want our final corpora to include the largest number of texts from the original ones.
2. **Female vs male authors balance**: we want the corpus of female and male authors to be as equally sized as possibile, in terms of global number of tokens.
3. **Size-per-decade balance**: we want a balanced distribution of tokens amongst each decade within the considered timespan, inside both the female and male authors corpus.
4. **Authors-per-decade balance**: we want the variety of both female and male authors to be represented within each decade, i.e. we want to have, in each decade, at least one book by each author, if any work by such author is present for such decade inside the original corpus.


The balancing process starts from a fundamental observation: in our original corpus, which has been built to be maximally inclusive (therefore comprehending the maximum number of available texts for each author relevant to our research), the texts written by female authors are generally shorter in size than books written by male authors. 

This is evident even in the bare count of global tokens for the female and male authors corpus:
* Female authors corpus:
  * Total number of words: 9458669
  * Number of books: 185
* Male authors corpus:
  * Total number of words: 14074486 
  * Number of books: 161

Despite the larger number of books written by female writers, the female authors corpus is considerably smaller in size, in terms of number of tokens, compared to the male authors corpus. 



???? **Size-per-author balance**: not met (neither decade-wise nor with respect to the whole corpus)