# Multi-scale Self-calibrated Network for Image Light Source Transfer
### Team: Wit-AI-lab 
#### Members: Yuanzhi Wang, Tao Lu, Yanduo Zhang, Yuntao Wu

It contains the codes to attend NTIRE 2021: Depth-Guided Image Relighting Challenge Track 1: One-to-one relighting

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
### Testing
- All test images are included in the `./dataset/NTIRE2021_TEST/test` folder.
- The model for testing is placed in `./checkpoints/best_model/latest_net_G.pth`
- Test the model:
```bash
python test.py
```
The test results will be saved to the folder: `./output`.


### Citation
If you find the code helpful in your resarch or work, please cite the following papers.
```
@inproceedings{mcn2021ntire,
    title     = {Multi-scale Self-calibrated Network for Image Light Source Transfer},
    author    = {Yuanzhi Wang and Tao Lu and Yanduo Zhang and Yuntao Wu},
    booktitle = {Proceedings of the IEEE Conference on Computer Vision and Pattern Recognition Workshops (CVPRW)},
    year      = {2021}
}
```
```
@inproceedings{elhelou2021ntire,
    title     = {{NTIRE} 2021: Depth-Guided Image Relighting Challenge},
    author    = {El Helou, Majed and Zhou, Ruofan and S\"usstrunk, Sabine and Timofte, Radu and others},
    booktitle = {Proceedings of the IEEE Conference on Computer Vision and Pattern Recognition Workshops (CVPRW)},
    year      = {2021}
}
```
