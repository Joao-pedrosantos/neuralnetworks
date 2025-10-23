# Exercise 4: Variational Autoencoder (VAE) on MNIST

## Notebook

!!! jupyter "Interactive Exercise"
   Here's the complete notebook.

   [:material-notebook: Open Exercise 1A Notebook](https://nbviewer.org/github/joao-pedrosantos/neuralnetworks/blob/main/docs/exercises/exercise4/vae_mnist.ipynb){ .md-button .md-button--primary }

   [:material-github: View Source on GitHub](https://github.com/joao-pedrosantos/neuralnetworks/blob/main/docs/exercises/exercise4/vae_mnist.ipynb){ .md-button }


## Conclusion

In this exercise, I implemented a Variational Autoencoder (VAE) model and trained it on the MNIST dataset.

During the first part of the exercise, I explored the theoretical foundations of VAEs, including the encoder-decoder architecture, the variational lower bound (ELBO), and the reparameterization trick. This helped me understand how VAEs learn latent representations and generate new data samples.

In the second part, I built a VAE from scratch using Python and PyTorch. I designed an encoder that maps input images to a latent space and a decoder that reconstructs images from latent vectors. The model was trained to minimize the reconstruction loss and the KL divergence, enabling it to generate realistic digit images.

In the third part, I experimented with the latent space by sampling from it to generate new images. I observed how the VAE could interpolate between digits and produce variations, demonstrating its generative capabilities. Additionally, I analyzed the learned latent representations and their clustering properties.

Finally, in the fourth part, I extended the VAE to a conditional version, conditioning on class labels to generate specific digits. This improved control over the generation process and highlighted the flexibility of VAEs for conditional generation tasks.

Overall, this exercise provided a deep understanding of Variational Autoencoders, from theory to implementation. It reinforced concepts in generative modeling, latent variable models, and probabilistic inference, showcasing the power of VAEs for unsupervised learning and data generation.