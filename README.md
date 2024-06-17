
<font size='5'>**SAM-CFFNet: SAM-Based Cross-Feature Fusion Network for Intelligent Identification of Landslides**</font>

Laidian Xi, [Junchuan Yu](https://github.com/JunchuanYu)☨, Daqing Ge, Yunxuan Pang, Ping Zhou, Changhong Hou, Yichuan Li, Yangyang Chen, Yuanbiao Dong

☨corresponding author


## To Do List
* **[2024.02.23]** Paper submission in review process.
* **[2023.03.17]** Dataset uploaded.
* **[2024.03.30]** Code test.
* **[2024.03.30]** Code realease.

## Dataset
The landslide datasets used in this study are all open source datasets, and the links to access the datasets and the literature are shown below
* Bijie Landlside Dataset: [Link](http://gpcv.whu.edu.cn/data/Bijie_pages.html),  [Paper](https://link.springer.com/article/10.1007/s10346-021-01694-6?fromPaywallRec=true).
* Landslide4Sense Dataset: [Link](https://github.com/iarai/Landslide4Sense-2022),  [Paper](https://ieeexplore.ieee.org/document/9944085).
* GVLM Dataset: [Link](https://github.com/zxk688/GVLM),  [Paper](https://www.sciencedirect.com/science/article/pii/S0924271623000242?dgcid=author).

You can also download our processed data directly:
[Baidu Disk](https://pan.baidu.com/s/19kVD7E5ECDAJgXcFGIfUtQ?pwd=4thn).链接：https://pan.baidu.com/s/12NeTM1GXoQnl24OgG_KbLA?pwd=71ne 
提取码：71ne 
--来自百度网盘超级会员V6的分享

## SAM-CFFNet
![](https://pic1.zhimg.com/100/v2-0c695da78b2119b960785047eaf78bc8_r.jpg 'SAM-CFFNet')
+ SAM-CFFNet backbone from [SAM](https://github.com/facebookresearch/segment-anything), some code references [Attention UNet](https://github.com/EdgarLefevre/Attention_Unet_Pytorch), [HRNet](https://link.zhihu.com/?target=https%3A//github.com/HRNet), [Deeplabv3+](https://github.com/yassouali/pytorch_segmentation/blob/master/models/deeplabv3_plus.py). SAM-CFFNet achieved the highest accuracy across three open-source remote sensing landslide datasets compared to other contrastive models.
+ Click the links below to download the checkpoint for the corresponding model type.

  - `ViT-L SAM`:  [Link](https://dl.fbaipublicfiles.com/segment_anything/sam_vit_l_0b3195.pth)   
    Save the file in your download directory:

    `/pretrained/sam_vit_l_0b3195.pth`

  - `SAM-CFFNET`:  [Baidu Disk](https://pan.baidu.com/s/12NeTM1GXoQnl24OgG_KbLA?pwd=71ne)   
    Save the file in your download directory:

    `/sam_cffnet_weight/{gvlm_best.pth.tar,BJL_best.pth.tar,L4S_best.pth.tar}`

+ The experimental code has been uploaded, and the training and validation of the model can be achieved through the ipynb file in it, and the supporting library information of the code is shown below:
<center>

|Package                    |Version|
|:----:  |:----: |
| GDAL                      |3.6.2|
| h5py                      |3.9.0|
| matplotlib                |3.7.2|
| numpy                     |1.24.1|
| opencv-python             |4.8.0.74|
| scipy                     |1.10.1|
| tensorboard               |2.10.1|
| tensorboardX              |2.6.2.2|
| torch                     |1.12.1|
| torchsummary              |1.5.1|
| torchvision               |0.13.1|
| tqdm                      |4.65.0|

</center>

## Acknowledgement
+ [SAM](https://github.com/facebookresearch/segment-anything).  SAM is the Segment Anything Model (SAM) proposed by Meta, which breaks through the boundaries of segmentation and greatly promotes the development of basic computer vision models.
+ [Attention UNet](https://github.com/EdgarLefevre/Attention_Unet_Pytorch). Attention mechanism enhances feature representation by focusing on informative regions during image segmentation.
+ [HRNet](https://link.zhihu.com/?target=https%3A//github.com/HRNet). High-Resolution Network maintains high-resolution feature maps throughout the network to capture fine details in images effectively.
+ [Deeplabv3+](https://github.com/yassouali/pytorch_segmentation/blob/master/models/deeplabv3_plus.py). DeepLabv3+ utilizes atrous spatial pyramid pooling and decoder module to achieve accurate semantic segmentation with multi-scale features.

If you're using SAM-CFFNet in your research or applications, please cite using this BibTeX:

```bibtex
@article{xi2024rs,
  title={SAM-CFFNet: SAM-Based Cross-Feature Fusion Network for Intelligent Identification of Landslides},
  author={Xi, Laidian and Yu, Junchuan and Ge,Daqing and Pang, Yunxuan and Zhou, and Ping and Hou, Changhong and Li, Yichuan and Chen, Yangyang and Dong, Yuanbiao },
  journal={Remote Sensing},
  year={2024}
}
```