# CGEC

## Codes for our work on Chinese Grammatical Error Correction.

## CGEC Dataset 

#### NLPCC 2018
|Split                   |# Sent   |# Token src.   | # Token tgt.  |
|------------------------|-----|-----|-----|
| Train|1.2 M|23.7 M| 25.0 M|
| Dev | 5.000| 84.5 K | 92.9 K|
| Test | 2.000 | 58.9 K | - |

## CGEC Performance

| System | Method | P | R | F<sub>0.5|
|------------------------|-----|-----|-----|-----|
|YouDao ([Kai et. al. 2018](http://tcci.ccf.org.cn/conference/2018/papers/EV39.pdf))|35.24|18.64|29.91|
|AliGM ([Zhou et. al. 2018](https://link.springer.com/chapter/10.1007/978-3-319-99501-4_10))|41.00|13.75|29.36|
|BLCU ([Ren et. al. 2018](https://link.springer.com/chapter/10.1007/978-3-319-99501-4_36))|47.63|12.56|30.57|
|PKU ([Zhao et. al. 2020](https://www.aaai.org/ojs/index.php/AAAI/article/view/5476))|44.36|22.18|36.97|
|CASIA|CSeq2Edit|  43.98| 22.65|37.01|

## CSC Dataset
#### SIGHAN CSC Dataset
| test set | # sent | # chars | # spelling erros (chars) | character set|genre|
|------------------------|-----|-----|-----|-----|-----|
SIGHAN 2015 |1,100|33,711|715|traditional|second-language learning|
SIGHAN 2014 |1,062|53,114|792|traditional|second-language learning|
SIGHAN 2013 |2,000|143,039|1,641|traditional|second-language learning|

| training set | # sent | # chars | # spelling erros (chars) | character set|genre|
|------------------------|-----|-----|-----|-----|-----|
SIGHAN 2015|3,174|95,220|4,237|traditional|second-language learning|
SIGHAN 2014|6,526|324,342|10,087|traditional|second-language learning|
SIGHAN 2013|350|17,220|350|traditional|second-language learning|

#### Synthetic training dataset

|  corpus | # sent | # chars | # spelling erros (chars) | character set|genre|
|------------------------|-----|-----|-----|-----|-----|
|Synthetic training dataset ([Wang et. al. 2018](https://www.aclweb.org/anthology/P19-1578)) | 271,329|12M|382,702|simplified|news|

## CSC Performance

|System | False Positive Rate| Detection Accuracy | Detection Precision| Detection Recall | Detection F1 | Correction Accuracy|Correction Precision|Correction Recall|Correction F1|
|-----|-----|-----|-----|-----|-----|-----|-----|-----|-----|
|CAS ([Zhang et. al. 2015](http://aclweb.org/anthology/W15-3107))|11.6|70.1|80.3|53.3|64.0|69.2|79.7|51.5|62.5|
|FASPell([Hong et. al. 2019](https://www.aclweb.org/anthology/D19-5522/))|-|74.2|67.6|60.0|63.5|73.7|66.6|59.1|62.6|
|Confusion-set([Wang et. al. 2019](https://www.aclweb.org/anthology/P19-1578/))|-|-|66.8|73.1|69.8|-|71.5|59.5|64.9|
|Soft-Masked BERT([Zhang et. al. 2020](https://www.aclweb.org/anthology/2020.acl-main.82))|-|80.9|73.7|73.2|73.5|77.4|66.7|66.2|66.4|