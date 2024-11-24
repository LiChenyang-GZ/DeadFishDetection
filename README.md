# Fish pond dead fish detection

The Project is based on YOLOV5, for individual vision detection practice.

## 1. About the Data

A total of 175 fish pond pictures were selected from the internet, of which 146 were taken as the training set and 29 as the test set. Labelimg was used to frame dead fish in the data set for training and validation. 

The picture of the fish pond is as follows:
![图片](https://github.com/user-attachments/assets/ac8042b4-c900-4bdb-8e71-650003e50df0)

## 2. Result

Using 146 training set pictures for training, 29 pictures for verification, the accuracy and recall rate are about 78%.
![图片](https://github.com/user-attachments/assets/cab76a97-8a5a-4092-a8c5-971604df27e2)


The model verification results are as follows. At present, the model has the ability to detect dead fish in fish ponds, whether the picture contains a large area of dead fish, or contains only one or two dead fish, the model can detect.

![val_batch0_pred](https://github.com/user-attachments/assets/e704a911-3173-4896-812d-77a7c09f8d21)

![val_batch1_pred](https://github.com/user-attachments/assets/084268c4-e3d4-48bd-b5ca-ee7181a7997c)


## 3. Potential Risk

1. The current training dataset is small in size, which may lead to over-adaptation of the model to the training data (overfitting), thus reducing its generalization ability in real applications.

2. The shooting angles and images of the pictures and the actual scene may be different, and the model may not be able to effectively adapt to the changes in the actual application, such as different shooting angles, lighting conditions, and background settings. Such differences may lead to lower detection accuracy of the model in real applications.

3. The current training dataset lacks images of live fish, and this category imbalance may lead to recognition bias in the model, reducing its adaptability and accuracy in diverse scenarios. There is a risk that the model misidentifies live fish as dead fish, especially when the model encounters scenarios with live fish in real-world applications.
