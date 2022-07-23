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

Model          |Resolution| mAP<sup>val<br>0.5 |CPU Latency<sup><br>(i5-10400) |ARM Latency<sup><br>(4xA76) | FLOPS      |   Params  | Model Size
:-------------:|:--------:|:-------:|:--------------------:|:--------------------:|:----------:|:---------:|:-------:
NanoDet-m      | 640*640 |   20.6   | **4.98ms**           | **10.23ms**          | **0.72G**  | **0.95M** | **1.8MB(FP16)** &#124; **980KB(INT8)**
**NanoDet-Plus-m** | 640*640 | **30.4** | **8.32ms**       | **19.77ms**          | **1.52G**  | **1.17M** | **2.3MB(FP16)** &#124; **1.2MB(INT8)**
YOLOv3-Tiny    | 640*640 |   16.6   | -                    | 37.6ms               | 5.62G      | 8.86M     |   33.7MB
YOLOv5s       | 640*640 |   28.4   | -                    | 44.39ms              | 4.5G       | 1.9M      |   3.8MB(FP16)
LUTDA        | 1152*320 |   30.4   | -                    | -                    | 1.8G       | -         |   -
MobileDet      | 320*320 |   25.6   | **8.32ms**                    | -                    | 0.9G       | -         |   -


 ## Acknowledgement

* [nanodet](https://github.com/RangiLyu/nanodet).
* [ FSACOCO](https://github.com/bitfsd/FSACOCO).
* Hubei University of Automotive Technology Driverless Racing Team
