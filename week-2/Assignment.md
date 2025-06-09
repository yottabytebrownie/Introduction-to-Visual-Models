#  Assignment:
## Part 1
Build and train your own CNN using CIFAR-10 and plot necessary graphs related to training the model.

## Part 2
Load a pretrained model (`VGG16`, `VGG19`, or `InceptionV3`). Evaluate its accuracy using weights of `imagnet` dataset only on CIFAR-100.
#### Problem You Will Face:
* **ImageNet has 1000 output classes**, while **CIFAR-10 has only 10**.
* Directly using the final layer of the pretrained model will not match CIFAR-10 labels.

Transfer Learning : Fine-Tune the chosen pre-trained model on CIFAR10 and then compare them

## Part 3
Make a 'pneumonia or normal classifier' using the kaggle dataset.
[kaggle link](https://www.kaggle.com/datasets/paultimothymooney/chest-xray-pneumonia)
Loading data in colab directly:
`
!pip install kaggle
!mkdir ~/.kaggle
!mv kaggle.json ~/.kaggle/
!kaggle datasets download -d paultimothymooney/chest-xray-pneumonia
!unzip chest-xray-pneumonia.zip`

Accuracy on testing data should be more than 60%



## In case you run out of GPU
Change the runtime type or use another google account.
