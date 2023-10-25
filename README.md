# DRG-generation-TAF
Code for the paper: Controlling Topic-Focus Articulation in Meaning-to-Text Generation using Graph Neural Networks.
## Environment (not sure)
- python>=3.8
- cuda==11.0
- gcc=9.4
- pytorch==1.7.1
- torchtext==0.8.1
- torch-geometric==1.5.0

```
#link about installing torch-geometric:
https://www.cnblogs.com/dive-into/p/16953369.html
https://pytorch-geometric.com/whl/
#link about installing gcc
https://zhuanlan.zhihu.com/p/371807723
```

## Data
```
# Download the data SBN-4.0.0 from PMB
# randomly spite data to train, dev, and test (1000)
# preprocess the SBN to sequential formats, such as the file "train.txt.graph.normal"
python SBN_process/sbn_preprocess.py -input_src data/train.txt
python SBN_process/sbn_preprocess.py -input_src data/test.txt
python SBN_process/sbn_preprocess.py -input_src data/dev.txt
```

## Process
```
sh preprocess.sh
```

## Train
```
sh train.sh
```

## Testn Set
```
sh decoder.sh
```

## Challenge Set
