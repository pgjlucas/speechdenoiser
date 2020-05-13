# Speech Denoiser
Development of an autoencoder able to denoise speeches by using both audio and video signals (lips movement)

# Library & tools
Keras | Tensorflow

# Autoencoder architecture
- Video encoder, fed with crops of mouths
- Audio encoder, fed with the mel frequency spectogram
- Latent vector transform
- Audio decoder
- Discriminator (for training)

# Dataset
GRID dataset

# Results



| Architecture  | MSE           | SNR           |
| ------------- | ------------- | ------------- |
| Everything    | 0.00280       | 0.00074       |
| No Video      | 0.00496       | 0.00104       | 
| No Discrim.   | 1.06589       | 0.00203       | 
| Just Audio    | 1.09894       | 0.00207       | 

