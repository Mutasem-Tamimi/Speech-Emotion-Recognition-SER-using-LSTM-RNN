
# Speech Emotion Recognition (SER) using LSTM-RNN

This project focuses on developing a Speech Emotion Recognition (SER) system, which is designed to identify and classify human emotions based on speech signals. The goal is to build a robust model that can accurately recognize emotions from speech data, using deep learning techniques.

## Datasets

The system is trained on two prominent datasets:

-   **TESS (Toronto Emotional Speech Set)**: A collection of emotion-annotated speech recordings featuring seven emotions.
-   **RAVDESS (Ryerson Audio-Visual Database of Emotional Speech and Song)**: A well-known dataset for emotion recognition tasks with speech samples labeled with different emotions.

## Emotion Classes

The model is designed to classify the following emotions:

-   Neutral
-   Calm
-   Happy
-   Sad
-   Angry
-   Fearful
-   Disgust
-   Surprised

## Preprocessing

The audio data undergoes the following preprocessing steps:

-   **Noise Reduction**: Removes background noise to enhance the clarity of the speech signals.
-   **Normalization**: Adjusts the audio signal amplitude to standardize the input.
-   **Silence Trimming**: Eliminates silence at the start and end of recordings to focus on the active speech segments.

## Data Augmentation

To improve model generalization and handle data scarcity, the following augmentation techniques are applied:

-   **Noise Augmentation**: Adds random noise to the audio signals.
-   **Time-Stretching**: Speeds up or slows down the audio while maintaining pitch.
-   **Pitch-Shifting**: Alters the pitch of the audio without changing its duration.
-   **Time-Shifting**: Shifts the audio signal slightly in time to introduce variety.

## Model Architecture

The core of the model is an **LSTM-RNN** (Long Short-Term Memory Recurrent Neural Network) architecture. This architecture is well-suited for sequential data like speech because of its ability to capture temporal dependencies in audio features.

## Results and Performance

The model's performance is evaluated based on the accuracy of emotion classification. Metrics such as confusion matrices and accuracy scores are used to assess its effectiveness.

## Tools and Libraries

-   Python
-   TensorFlow/Keras
-   Librosa (for audio processing)
-   Scikit-learn (for data handling and evaluation)
-   Seaborn
