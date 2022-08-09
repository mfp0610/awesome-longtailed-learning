# LT Survey: LADE

LADE: Disentangling Label Distribution for Long-tailed Visual Recognition. (CVPR 2021)

[paper](https://arxiv.org/abs/2012.00321)

## Usage

For CIFAR-100 with imbalance ratio 0.1, training LADE:

```bash
python main.py --seed 1 --cfg config/CIFAR100_LT/lade.yaml --exp_name lade2021/cifar100_imb0.01_lade --cifar_imb_ratio 0.1 --remine_lambda 0.01 --alpha 0.1 --gpu 0
```

Evaluation for CIFAR-100:

```bash
./notebooks/cifar100-shift-calib.ipynb
```
