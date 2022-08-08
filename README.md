# GAN Video Colorization
We train three different models to colorize a grayscale video. 
- Colorization Net -> A pretrained resnet with upsampling as generator, PATCHGan as discrimainator, and trained on BCE, MSE, L1, and Perceptual Loss. 
- Colorization with U-Net -> An U-Net encoder-decoder acts as generator, PATCHGan as discrimainator, and model is trained using NOGan methodlogy where generator and discriminator are pre-trained separately before adversarial training is done.
- Colorization with U-Net and Wasserstein Loss -> Addition of Wasserstein Loss on second model.

A output sample is store in output folder with results from different models. Please refer to report file GANVideoColorization.pdf for detailed explanation on the architecture, training regime, and results of the models created.

The Train file for each model is in their respective folder. Once model are trained, the test code for all of them can be found in test.ipynb.

