# Multi-scale Self-calibrated Network for Image Light Source Transfer
### Team: Wit-AI-lab 
#### Members: Yuanzhi Wang, Tao Lu, Yanduo Zhang, Yuntao Wu

It contains the codes to attend NTIRE 2021: Depth-Guided Image Relighting Challenge Track 1: One-to-one relighting

Paper link: [CVPR2021W](https://openaccess.thecvf.com/content/CVPR2021W/NTIRE/html/Wang_Multi-Scale_Self-Calibrated_Network_for_Image_Light_Source_Transfer_CVPRW_2021_paper.html)

## Prerequisites
- Linux (Ubuntu 1604 or Windows 10)
- Anaconda
- Python 3.7
- NVIDIA RTX2080Ti GPU (11G memory or larger) + CUDA10.2 + cuDNN
- PyTorch1.5.0 
- dominate
- kornia 0.2.0
- lpips-pytorch

## Getting Started
### Installation
- Create a conda virtual environment
```bash
conda create -n MCN python=3.7
```
- Install PyTorch
```bash
conda install pytorch==1.5.1 torchvision==0.6.1 cudatoolkit=10.2 -c pytorch
```
- Install dominate
```bash
pip install dominate
```
- Install kornia
```bash
pip install kornia==0.2.0
```
- Install lpips-pytorch
```bash 
pip install git+https://github.com/S-aiueo32/lpips-pytorch.git
```
### Pre-trained model
Please download pre-trained model
Google drive link: [Download](https://drive.google.com/file/d/1PFD_uidOlqg5xqD9Wsz3RWX8Z4CmwT3s/view?usp=sharing)

### Testing
- Two test images are included in the `./dataset/NTIRE2021_TEST/test`
- Please place the pre-trained model in `./checkpoints/best_model/latest_net_G.pth`
- Test the model:
```bash
python test.py
```
The test results will be saved to the folder: `./output`.

### Training
The training code will be released soon

### Citation
If you find the code helpful in your resarch or work, please cite the following papers.
```
@InProceedings{Wang_2021_CVPR,
    author    = {Wang, Yuanzhi and Lu, Tao and Zhang, Yanduo and Wu, Yuntao},
    title     = {Multi-Scale Self-Calibrated Network for Image Light Source Transfer},
    booktitle = {Proceedings of the IEEE/CVF Conference on Computer Vision and Pattern Recognition (CVPR) Workshops},
    month     = {June},
    year      = {2021},
    pages     = {252-259}
}
```

## Acknowledgments
This code borrows heavily from [DRN](https://github.com/WangLiwen1994/DeepRelight).
