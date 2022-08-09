# Lt Survey: TADE

TADE: Test-Agnostic Long-Tailed Recognition 

[paper](https://arxiv.org/pdf/2107.09249v2.pdf)

## Usage

### Training

To train the expertise-diverse model, run this command:
```bash
python train.py -c configs/config_cifar100_ir100_tade.json
```
One can change the imbalance ratio from 100 to 10/50 by changing the config file.

### Evaluate
To evaluate expertise-diverse model on the uniform test class distribution, run:
```bash
python test.py -r checkpoint_path
``` 

To evaluate expertise-diverse model on agnostic test class distributions, run:
```bash
python test_all_cifar.py -r checkpoint_path
``` 

#### Test-time training
To test-time train the expertise-diverse model for agnostic test class distributions, run:
```bash
python test_train_cifar.py -c configs/test_time_cifar100_ir100_tade.json -r checkpoint_path
``` 
One can change the imbalance ratio from 100 to 10/50 by changing the config file.
