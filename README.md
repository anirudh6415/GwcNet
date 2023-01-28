# GwcNet
This is the implementation of the paper Group-wise Correlation Stereo Network
# How to use
## Environment
python 3.6
Pytorch >= 0.4.1
# Data Preparation
Download Scene Flow Datasets, KITTI 2012, KITTI 2015

# Training
## Scene Flow Datasets

run the script ./scripts/sceneflow.sh to train on Scene Flow datsets. Please update DATAPATH in the bash file as your training data path.

## KITTI 2012 / 2015

run the script ./scripts/kitti12.sh and ./scripts/kitti15.sh to finetune on the KITTI 12/15 dataset. Please update DATAPATH and --loadckpt as your training data path and pretrained SceneFlow checkpoint file.

# Evaluation
run the script ./scripts/kitti12_save.sh and ./scripts/kitti15_save.sh to save png predictions on the test set of the KITTI datasets to the folder ./predictions.

# Pretrained Models
Scene Flow KITTI 2012/2015

# Citation
If you find this code useful in your research, please cite:

@inproceedings{guo2019group,
  title={Group-wise Correlation Stereo Network},
  author={Guo, Xiaoyang and Yang, Kai and Yang, Wukui and Wang, Xiaogang and Li, Hongsheng},
  booktitle={Proceedings of the IEEE Conference on Computer Vision and Pattern Recognition},
  pages={3273--3282},
  year={2019}
}
# Acknowledgements
Thanks to Jia-Ren Chang for opening source of his excellent work PSMNet. Our work is inspired by this work and part of codes in models are migrated from PSMNet.
Thanks to Xiaoyang Guo for the github Repo https://github.com/xy-guo/GwcNet/commit/0987074f48b098c6e975a58ca5aacf233b0fb0eb.
