# Efiicient_Resnet_with_CutMix_and_Mixup
Mini Project developed for Deep Learning course at NYU (Spring 24)

Our best model with accuracy of 97.08 % on CIFAR-10 dataset is in final_run.ipynb. The notebook can be run end to end to train the model on CIFAR-10 train dataset and get similar results. Model weights to replicate our results can be downloaded [here](https://drive.google.com/file/d/1qU-ccEGVzH45_1eavXP91abR70-d7WVt/view?usp=drive_link)

In final_run.ipynb the Efficient ResNet model was trained on CIFAR-10 training data with CutMix and MixUp for 200 epochs. In trial_run.ipynb same model was trained but without CutMix and MixUp for 200 epochs, then it was further finetuned for 130 epochs with CutMix and MixUp. First case gave us better accuracy on test data of 97.08 % whereas in the second case it was 96.07 %.

Efficient ResNet architecture was adapted from it's official github [repo](https://github.com/Nikunj-Gupta/Efficient_ResNets/tree/master), all the hyperparameters were kept same as their best case model. Their peak accuracy on test data was 96.04 % using same model, so by using additional data augmentation the model was able to generalize better.
