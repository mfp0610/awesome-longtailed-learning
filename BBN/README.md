# LT Survey: BBN

BBN: Bilateral-Branch Network with Cumulative Learning for Long-Tailed Visual Recognition. (CVPR2020 Oral)

[paper](https://arxiv.org/abs/1912.02413) 

## Main requirements

* **torch == 1.0.1**
* **torchvision == 0.2.2_post3**
* **tensorboardX == 1.8**
* **Python 3**

## Usage

```bash
# To train long-tailed CIFAR-10 with imbalanced ratio of 50:
python main/train.py  --cfg configs/cifar10.yaml     

# To validate with the best model:
python main/valid.py  --cfg configs/cifar10.yaml

# To debug with CPU mode:
python main/train.py  --cfg configs/cifar10.yaml   CPU_MODE True
```

You can change the experimental setting by simply modifying the parameter in the yaml file.