# multi-view-vae
Joint VAE for modeling MNIST and SHVN datasets



Explain how the model was trained. The notebook is configured for Adam, learning rate \(10^{-3}\), batch size 32, 20 epochs, latent dimension 20, and observation variance 0.1. Mention the 10% validation split and selection of the checkpoint with the lowest validation loss. Report the settings actually used in the final run.

Clarify the three training configurations: both images available, MNIST only, and SVHN only. Each configuration reconstructs both images; the three losses are averaged. Your existing final paragraph introduces this but never explicitly lists the configurations.

Present training performance. Briefly discuss training/validation loss curves and final held-out performance, using actual run outputs.

Show reconstructions. Compare original MNIST and SVHN images with their reconstructed versions and comment on quality.

Show generation from the prior. Sample \(z\sim\mathcal N(0,I)\), decode it into both domains, and discuss image quality and whether the digits agree.

Show cross-domain generation in both directions: MNIST → SVHN and SVHN → MNIST. Explain whether digit identity is preserved.

Include t-SNE. Plot the shared latent representations, colour by digit, and discuss clustering and alignment between the input configurations.

Finish with a short conclusion and the code link. Summarize what worked, limitations, and possible improvements.