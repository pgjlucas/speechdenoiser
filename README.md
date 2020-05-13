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

