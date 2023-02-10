# D-SRA-Pytorch

This repository implements a GAN based model for super resolution of flow images captured by high-speed camera. The images are first converted to low resolution by a learned degradation network, which is trained in unsupervised setting. Then like a typical SRGAN, the network is trianed in paired setting and finally stored to give inference.
 
 ## Architecture
 Degradation model -------------------> contains all codes of degradation model, including:  train_De.py, predict_De.py
 
 SRA model  ----------------------->contains all codes of SRA model, including:  SRA_train.py, SRA _predict.py
 
 data ---------------------> contains all data of D-SRA model training and testing, including LRHF, HRLF for Degradation model, LRHF and LRLF for SRA model
 

## How to Train
run main file
#training of Degradation model:
```bash
python train_De.py   
```
#training of SRA model:
```bash
python SRA_train.py   
```


## How to Predict
#testing of Degradation model:
```bash
python predict_De.py   
```
#testing of SRA model:
```bash
python SRA_predict.py   
```

Note: All the file path in original code have been repalced by 'your path', so you should enter you file path or filename before running the code. 
There is only partial data in the file, if you want to obtain all the data, please contact the author by email.
Due to copyright restrictions, it can only be used for research, not for commercial use.
