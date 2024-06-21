# RempahRasaML

## Introduction
Repository contains image classification models with 31 classes. The models are trained using custom CNN methods and transfer learning to recognize Indonesian spices images. Five architectures that we use for transfer learning includes: InceptionV3, Xception, DenseNet121, EfficientNetV2B0, and MobileNetV3. After the training, we find out that the model with the highest accuracy is DenseNet121 architecture with 94.37% accuracy on test dataset.

## Spices Classification Model
### Dataset
- https://www.kaggle.com/datasets/albertnathaniel12/indonesian-spices-dataset

There are total 6510 data and 31 classes of indonesian spices images including:
1. adas
2. andaliman
3. asam jawa
4. bawang bombai
5. bawang merah
6. bawang putih
7. biji ketumbar
8. bukan rempah
9. bunga lawang
10. cengkeh
11. daun jeruk
12. daun kemangi
13. daun ketumbar
14. daun salam
15. jahe
16. jinten
17. kapulaga
18. kayu manis
19. kayu secang
20. kemiri
21. kemukus
22. kencur
23. kluwek
24. kunyit
25. lada
26. lengkuas
27. pala
28. saffron
29. serai
30. vanili
31. wijen

### Model Architecture
![transfer_learning_model_custom (1)](https://github.com/RempahRasa/RempahRasaML/assets/127374698/9e78d713-2d41-4f57-98fa-7a06cdcaa9d4)

### Training and Evaluation
#### Pretraining
- Before training, we have splitted the data into 70% for training, 15% for validation, and 15% for test.
- Visualization some of the data
  ![image](https://github.com/RempahRasa/RempahRasaML/assets/127374698/74229711-d54b-4f28-825e-3e078d5cb85d)

#### Training
- We have trained the model and after 50 epochs, we obtained loss: 0.1228 and accuracy 96.44% for training. For validation, the val_loss is 0.3062 with 93.35% accuracy.
  ![image](https://github.com/RempahRasa/RempahRasaML/assets/127374698/cfa62683-a54e-43be-9859-344d0a273d64)

#### Evaluation
- We also have evaluated the model on test set, and achieved loss 0.23866 with 94.37% accuracy.
  ![image](https://github.com/RempahRasa/RempahRasaML/assets/127374698/2249f8fb-e6d3-449f-ae0e-fa6e880008fd)
- Visualization of data prediction
  ![image](https://github.com/RempahRasa/RempahRasaML/assets/127374698/0f8577b2-dbc1-45d4-915a-5c50e4af5e7b)


## Spices Classification model file (.h5 and tfjs for deployment)
https://drive.google.com/drive/folders/1axCQ-LzEvcT-2hm-bzMSf215pR7z8iWe?usp=sharing
