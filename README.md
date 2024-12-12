## Description :
this deep learning model was made to classify skin face disease including acne, wrinkle, and redness using tensorflow we build CNN model that also implement transfer learning and fine tuning

## Packages and Library :
- os
- numpy
- pandas
- seaborn
- matplotlib.pyplot
- tensorflow

## Dataset We Used : 
https://www.kaggle.com/datasets/panupongsingdee/acneclearcomedo-dataset

## Model Architecture :
![image](https://github.com/user-attachments/assets/e4ace590-a83d-4df4-b03f-a3b85169a414)
### What We Used In Our Model:
1. **Transfer Learning**:
   - Menggunakan **MobileNetV2** sebagai backbone model.

2. **Pooling**:
   - **GlobalAveragePooling2D** digunakan untuk merangkum fitur dari MobileNetV2 menjadi vektor.

3. **Fully Connected Layer**:
   - Dense layer dengan **128 neuron** menggunakan fungsi aktivasi **ReLU**.

4. **Dropout**:
   - Dropout sebesar **0.5** digunakan untuk mencegah overfitting.

5. **Output Layer**:
   - Dense layer dengan **4 neuron** menggunakan fungsi aktivasi **Softmax** untuk prediksi kelas.

## Training Result :
![WhatsApp Image 2024-11-28 at 6 03 32 PM](https://github.com/user-attachments/assets/73b085bf-b077-4e73-a27c-c4aaa1d44b82)
### Training Parameter :
- Optimizer: Adam
- Learning Rate: 0.0001
- Loss Function: Categorical Crossentropy
- Batch Size: 32
- Epochs: 50
- Validation Split: 20%
### Accuracy :
- Training Accuracy: 0.9156%
- Validation Accuracy: 0.9060%
- Training Loss: 0.2412%
- Validation Loss: 0.2676%

### Test Evaluate :
- Test accuracy : 0.8833%
- Test loss : 0.3522%

## Confusion Matrix :
![output](https://github.com/user-attachments/assets/c8d1352a-8f5d-4d45-8583-0ee739d707b3)
