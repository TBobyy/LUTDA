# LUTDA
  Lightweight driverless target detection algorithm is applied to driverless data sets such as Kitti and fsacoco
  
# Prerequisites

```
$conda create -n LUTDA python=3.8 -y
$conda activate LUTDA
$conda install pytorch==1.8.0 torchvision==0.9.0 torchaudio==0.8.0 cudatoolkit=11.1 -c pytorch -c nvidia
$pip install Cython termcolor numpy tensorboard pycocotools matplotlib pyaml opencv-python tqdm pytorch-lightning torchmetrics
```
## Benchmarks

Model          |Resolution| mAP<sup>val<br>0.5 |GPU Latency<sup><br>(RTX 3060) | FLOPS      |   Params  | Model Size
:-------------:|:--------:|:--------:|:--------------------:|:----------:|:---------:|:-------:
NanoDet-Plus-m | 640*640  |   84.4   |                      | **1.52G**  | **1.17M** | -
YOLOv3-Tiny    | 640*640  |   16.6   | -                    | 5.62G      | 8.86M     |33.7MB
YOLOv5s        | 640*640  |   92.8   | -                    | 16.4G       | 1.9M      |3.8MB
**LUTDA**      | 1152*320 | **93.6** | -                    | 4.8G       | -         |-


 ## Acknowledgement

* [nanodet](https://github.com/RangiLyu/nanodet).
* [ FSACOCO](https://github.com/bitfsd/FSACOCO).
* Hubei University of Automotive Technology Driverless Racing Team
