# BNL Covid-19 Drug Docking Dataset 2021


## To validate the data files
```
sha256sum train.tar.gz 
a7c3ab51a37048f23332337d05e9b5d75e76caca5ad31a8c5e505c1a2fae0404
sha256sum test.tar.gz
d563afaae3e99fcd566daae6c9c40c851750620d15f52850976723e6f31b3417
```

## To extract the data
```
tar xfvz train.tar.gz 
tar xfvz test.tar.gz
```

## sample code to load data
```
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
Test dataset has the same structure but filled with `NaN`.

## Contact

If you have any questions, feel free to contact us BC3D_2021[at]protonmail.com.

