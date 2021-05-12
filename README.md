# Plant Disease Detection
Plant disease detection using Keras on <b> [Plant Village](https://www.kaggle.com/emmarex/plantdisease) </b> dataset. 

### VGG-16 model
I’ve performed transfer learning by making use of the pre-trained model. Deep learning networks learn in a hierarchical fashion, i.e., they learn the high level features in the initial layers, and then the more specific features in the later layers. So, using the initial layers of the pre-trained model, and then adding other trainable layers on the top of it gave good results. <br> <br>
Here, I've freezed the convolutional base layers and trained the four other dense layers that were added. I’ve used binary cross entropy loss function and Adam optimizer. With this architecture, I’ve performed the classification. In addition to this, a further improvement could’ve been fine tuning, by unfreezing the entire model and re-training which could adapt the pre-trained features to the new data. <br>


<b>Optimizer</b> : Adam <br>
<b>Loss Function</b> : Binary Cross entropy 

## Results obtained

![Alt text](/vggAcc.png?raw=true "Optional Title")

![Alt text](/vggAcc2.png?raw=true "Optional Title")

<b>Accuracy on the test data</b> : 86.80%
