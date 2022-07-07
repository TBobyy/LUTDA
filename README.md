# LUTDA
  Lightweight driverless target detection algorithm is applied to driverless data sets such as Kitti and fsacoco
  
# Prerequisites

```
$conda create -n LUTDA python=3.8 -y
$conda activate LUTDA
$conda install pytorch==1.8.0 torchvision==0.9.0 torchaudio==0.8.0 cudatoolkit=11.1 -c pytorch -c nvidia
$pip install Cython termcolor numpy tensorboard pycocotools matplotlib pyaml opencv-python tqdm pytorch-lightning torchmetrics
```


 ## Acknowledgement

* [nanodet](https://github.com/RangiLyu/nanodet).
* [ FSACOCO](https://github.com/bitfsd/FSACOCO).
* Hubei University of Automotive Technology Driverless Racing Team
