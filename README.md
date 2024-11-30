# Sentiment Analysis from Audio Data

This is a Machine Learning classification model designed to perform sentiment analysis on human audio data.

## Audio Characteristics

- **Frequency**: The number of oscillations per second in the audio signal.
- **Pitch**: The perceived frequency of the sound, indicating whether it's high or low.
- **Amplitude**: The loudness or intensity of the sound.
- **Tone**: The quality or character of the sound.
- **Sampling Rate**: The number of samples of audio per second.
- **Bit Depth**: The number of bits used to represent each sample.
- **Noise**: Unwanted sound that interferes with the clarity of the signal.
- **Duration**: The length of the audio recording.

## Fourier Transform

The **Fourier Transform** is a mathematical tool that decomposes a function (such as a sound wave) into its constituent frequencies. It transforms a time-domain signal into the frequency domain, showing how much of each frequency is present in the original signal.

For audio, this means converting a waveform (amplitude over time) into a frequency spectrum (amplitude of different frequencies).

## Methods to Visualize Audio Data

- **Waveform / Waveplot**: Useful for understanding the overall shape of the audio waveform, such as loud or quiet sections.
- **Spectrogram**: Visualizes the frequency of the audio over time (time vs. frequency, with amplitude as color intensity).
- **Melspectrogram**: The frequency axis is transformed into the Mel scale, compressing higher frequencies to better match how humans perceive sound.
- **MFCC (Mel-frequency Cepstral Coefficients)**: These are a set of features (typically 12-20) that represent the most important aspects of the Mel spectrogram, derived through a process of FFT → Mel filtering → Log scaling → DCT.

## Augmentation of Audio Data

To enhance the dataset and improve the model's generalization, audio data can be augmented in several ways:
- Adding noise
- Stretching the audio
- Shifting the audio
- Changing the pitch