# Audio Classification using Deep Learning

This project aims to classify audio files into different categories using deep learning techniques. The classification task is performed on the UrbanSound dataset, which contains various urban sounds across different categories.

## Dataset

The UrbanSound dataset consists of 10 sound categories, including air conditioner, car horn, children playing, dog bark, drilling, engine idling, gun shot, jackhammer, siren, and street music. Each category contains audio recordings captured in urban environments.

## Workflow

1. **Data Loading and Visualization**: The audio files are loaded using Librosa, and sample audio waveforms are visualized using Matplotlib.

2. **Feature Extraction**: Mel-frequency cepstral coefficients (MFCCs) are extracted from the audio files. MFCCs are commonly used as features in audio processing tasks due to their effectiveness in representing the characteristics of audio signals.

3. **Data Preprocessing**: The extracted features are combined with their corresponding labels. Label encoding is applied to convert categorical labels into numerical format, and the dataset is split into training and testing sets.

4. **Model Building**: A neural network model is constructed using TensorFlow's Keras API. The model architecture consists of several dense layers with rectified linear unit (ReLU) activation functions and a softmax output layer.

5. **Model Training**: The model is trained on the training data using the Adam optimizer and categorical cross-entropy loss function.

6. **Model Evaluation**: After training, the model's performance is evaluated on the test set using accuracy as the evaluation metric.

7. **Inference**: The trained model is used to predict the class of new audio files. MFCCs are extracted from the new audio files, and the model predicts the corresponding category.


## Results

The trained model achieves an accuracy of 81% on the test set, demonstrating its effectiveness in classifying urban sounds.

## Future Work

- Explore other deep learning architectures for audio classification.
- Fine-tune hyperparameters to improve model performance.
- Investigate techniques for handling imbalanced classes in the dataset.
