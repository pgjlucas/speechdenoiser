# Speech Denoiser
Development of an autoencoder able to denoise speeches by using both audio and video signals (lips movement)

# Library & tools
Keras | cv2 | Librosa

# Autoencoder architecture
- Video encoder, fed with crops of mouths
- Audio encoder, fed with the mel frequency spectogram of the audio, where a Gaussian noise was added
- Latent vector transform
- Audio decoder
- Discriminator (for training)

# Dataset
GRID dataset

# Results
The criteria to evaluate our model were MSE and SNR. 
On the table below, we studied the effects of the different parts of our model.
The results were obtained for the following settings:
- Training & testing gaussian noise level : 0.5
- Epochs : 20

| Architecture  | MSE | SNR |
| ------------- | ------------- |------------- |
| Everything | 0.00280 | 0.00074  |
| No Video    | 0.00496  | 0.00104  |
| No Discrim.     | 1.06589   | 0.00203 |
| Just Audio   | 1.09894  | 0.00207 |


More info on the [pdf paper](https://github.com/pgjlucas/speechdenoiser/blob/master/Paper.pdf).
