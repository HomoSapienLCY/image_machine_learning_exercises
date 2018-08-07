# image_machine_learning_exercises

Some implementation ideas are learned from:
- https://github.com/jhkim89/PyramidNet
- https://github.com/hysts/pytorch_image_classification
- https://github.com/kuangliu/pytorch-cifar
- https://github.com/xternalz/WideResNet-pytorch

During the implementation, many thanks for sharing their code

The accuracies of PreActResNet, WideResNet and PyramidNet on the [Cifar-10](https://www.cs.toronto.edu/~kriz/cifar.html) dataset matches the numbers in the paper.

On the [BreakHis](https://web.inf.ufpr.br/vri/databases/breast-cancer-histopathological-database-breakhis/) dataset, the accuracy is ~93-95% on 30% testing data (400X) using PreActResNet18.

To run a model on the BreakHis dataset:
- 1 download the BreakHis dataset and put it in a folder in the location ../Datasets
- 2 bash run_Net.sh
- 3 after the first run, you can change the run_Net.sh file into: python Histology_Main.py 1 0.5 0 0.1 1 1, to save data reading time

To run the Cifar-10 dataset:
- 1 download the Cifar-10 dataset and put it in a folder in the location ../Datasets
- 2 python Cifar_Main.py "initial learning rate" 1 (initial learning rate of 0.1 can replicate the accuracy mentioned above)
