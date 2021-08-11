# CaraNet: Context Axial Reverse Attention Network for Small Medical Objects Segmentation
<div align=center><img src="https://github.com/AngeLouCN/CaraNet/blob/main/figures/caranet.jpg" width="1000" height="450" alt="Result"/></div>
This repository contains the implementation of a novel attention based network (CaraNet) to segment the polyp (CVC-T, CVC-ClinicDB, CVC-ColonDB, ETIS and Kvasir) and brain tumor (BraTS). The CaraNet show great overall segmentation performance (mean dice) on polyp and brain tumor, but also show great performance on small medical objects (small polyps and brain tumors) segmentation. 

**The technique report is coming soon!**

## Architecture of CaraNet
### Backbone
We use **Res2Net** as our backbone.

### Context module
We choose our CFP module as context module, and choose the dilation rate is **8**. The architecture of **CFP module** as shown in following figure:
<div align=center><img src="https://github.com/AngeLouCN/CFPNet/blob/main/figures/cfp module.png" width="800" height="300" alt="Result"/></div>

### Axial Reverse Attention
As shown in architecture of CaraNet, the Axial Reverse Attention (A-RA) module contains two routes: 1) Reverse attention; 2) Axial-attention.

## Installation
- Enviroment: Python 3.6;
- Install some packages:

```
conda install pytorch==1.1.0 torchvision==0.3.0 cudatoolkit=10.0 -c pytorch
```
```
conda install opencv-python pillow numpy matplotlib
```
- Clone this repository
```
git clone https://github.com/AngeLouCN/CaraNet
```

