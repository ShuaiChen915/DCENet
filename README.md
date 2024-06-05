# DCENet: A tiny Object Detection Network for UAV images Based on Deformable Cross-Attention and Enhanced Classifier
This is the codebase of my journal paper DCENet: A Tiny Object Detection Network for UAV images Based on Deformable Cross-Attention and Enhanced Classifier module
# Model Architecture
![image](https://github.com/ShuaiChen915/DCENet/assets/126312301/501ebcd4-389e-47a7-8648-02b3af2163be)
# Detection stage Weights
| Name   | Dataset      | Input Size | Epochs | mAP  | Download(.pth)                                                       |
|--------|--------------|------------|--------|------|----------------------------------------------------------------------|
| DCENet | VisDrone-DET | 1920*1920  | 80     | 36.0 | [BaiduYun](https://pan.baidu.com/s/1WoioJIWALZFdrI0nzyxtOg?pwd=ck3w) |
| DCENet | UAVDT        | 1024*1024  | 36     | 27.5 | [BaiduYun](https://pan.baidu.com/s/1ZvZMfTCvpnht6oCed5rk0A?pwd=cnif) |

# Enhanced Classifier Weights
The VisDrone and UAVDT datasets are cropped into numerous image patches according to their ground truth. Subsequently, CSRM is employed to upscale the resolution, thereby forming classification datasets. ResNet-34 is then trained separately on these two classification datasets. The two datasets and model weights are provided below.
| Name      | Classifier Dataset                                                       | Input Size | Epochs | Download(.pth)                                                       |
|-----------|--------------------------------------------------------------------------|------------|--------|----------------------------------------------------------------------|
| ResNet-34 | [VisDrone-DET](https://pan.baidu.com/s/1PLY0V9-rLJ158JmOrSzU2g?pwd=3h6l) | 224*224    | 25     | [BaiduYun](https://pan.baidu.com/s/1W6sdX0YOMlODF8ngRR6gyw?pwd=sw8z) |
| ResNet-34 | [UAVDT](https://pan.baidu.com/s/190V9Tzo_STobk94nkPKJGw?pwd=k42d)        | 224*224    | 25     | [BaiduYun](https://pan.baidu.com/s/1rQcUvwz5taBjl5EWn5mFFQ?pwd=501b) |

