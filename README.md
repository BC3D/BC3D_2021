# BNL Covid-19 Drug Docking Dataset 2021

## Updates 09/06/2023:

* Uploaded the test partition with ground truth `test_w_gt.tar.gz`.
* To learn more about this dataset, please refer to our publication [arxiv:2308.01921](https://arxiv.org/abs/2308.01921).
* This dataset has been used as a challenge in 2021 [IEEE Healthcare Summit (IHS) COVID-19 Data Hackathone.](https://healthcaresummit.ieee.org/data-hackathon/ieee-covid-19-bioinformatics-single-cell-sequencing-drug-target-challenge/)


## To validate the data files

```bash
sha256sum train.tar.gz 
a7c3ab51a37048f23332337d05e9b5d75e76caca5ad31a8c5e505c1a2fae0404
sha256sum test.tar.gz
d563afaae3e99fcd566daae6c9c40c851750620d15f52850976723e6f31b3417
sha256sum test_w_gt.tar.gz
43ef84923768380c0ecfc07092d49f2715ef592a9b4eeed39fea216e7097c5a4
```

## To extract the data

```bash
tar xfvz train.tar.gz 
tar xfvz test.tar.gz
tar xfvz test_w_gt.tar.gz
```

## Sample code to load data

```python
import pandas as pd
df = pd.read_csv("train.csv")
print(df.columns.tolist())
['SMILES',
 '3CLPro_pocket1',
 'ADRP-ADPR_pocket1',
 'ADRP-ADPR_pocket5',
 'ADRP_pocket1',
 'ADRP_pocket12',
 'ADRP_pocket13',
 'COV_pocket1',
 'COV_pocket2',
 'COV_pocket8',
 'COV_pocket10',
 'NSP9_pocket2',
 'NSP9_pocket7',
 'NSP15_pocket1',
 'ORF7A_pocket2',
 'PLPro_chainA_pocket3',
 'PLPro_chainA_pocket23',
 'PLPro_pocket6',
 'PLPro_pocket50']
```
The dataset containing 18 targets.
Test (`test.tar.gz`) dataset has the same structure but filled with `NaN` for scores.
Test-with-groundtruth (`test_w_gt.tar.gz`) contains the scores.

## Contact

If you have any questions about the dataset, feel free to contact us {yren,hvandam,dlu}[at]bnl.gov.
(The previous contact email was BC3D_2021[at]protonmail.com for the data challenge.)

