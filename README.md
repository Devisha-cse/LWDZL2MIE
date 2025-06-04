# LWDZL2MIE
A Lightweight Multi-Image Encryption Scheme using Dynamic Chaotic SBox-PBox based Substitution Permutation Network
Creative Commons Attribution-NonCommercial 4.0 International

# 🛡️ Lightweight Multi-Image Encryption Scheme  
## Using Dynamic Chaotic SBox-PBox Based Substitution-Permutation Network

This project implements a **lightweight multi-image encryption scheme** using a dynamic **chaotic Substitution-Permutation Network (SPN)** architecture. It includes an interactive dashboard built with **Plotly Dash**, allowing real-time visualization of entropy trajectories, chaotic S-Boxes, and lattice-based P-Box transformations.

> **Note:** This project is released under a **non-commercial license** (CC BY-NC 4.0). Commercial use is strictly prohibited.

---

## 📸 Dashboard Features

- 📈 **Entropy Trajectory Graph**: Bounded entropy curve showing encryption randomness
- 🔲 **512x512 S-Box Heatmap**: Real-time substitution dynamics via chaotic mapping
- 🌀 **3D P-Box Trajectory**: Visualization of chaotic permutation paths
- 🌈 **Fluorescent Color Scheme**: Designed for high-contrast scientific illustration

---

## 🚀 Quick Start

### 1. Clone the repository

```bash
git clone https://github.com/your-username/your-repo-name.git
cd your-repo-name

QA_CL_SPN_Project/
├── README.md
├── LICENSE
├── main_pipeline.m                      # Main script: load, encrypt, decrypt, visualize
├── qa_cl_spn_encrypt.m                 # Encryption function
├── qa_cl_spn_decrypt.m                 # Decryption function (inverse of encryption)
├── compose_image_grid.m                # Utility: 8x4 or custom image grid
├── visualize_decrypted_composite.m     # Optional: standalone decrypted image grid
├── quantum_aware_tensor_sampling.m     # Constructs 32x32 tensor of images (or simplified 32 batch)
├── qa_encryption_analysis.m            # NPCR, UACI, CCA, SSIM, PSNR, pixel distribution analysis
├── data/
│   ├── original_images/                # 32 PNG images (18901.png to 18932.png)
│   ├── encrypted_grid.png
│   └── decrypted_grid.png
├── results/
│   ├── npcr_uaci_results.mat
│   ├── cca_3Dplots.png
│   ├── ssim_psnr_scores.txt
│   ├── decrypted_image_composite.png
│   └── pixel_distribution_comparison.png
├── docs/
│   ├── citation.txt
│   └── methodology_summary.pdf
\📄 README Section (Add This to Existing README.md)
🔬 Quantum Tensor Sampling & Analysis

    quantum_aware_tensor_sampling.m: Prepares a 32-image tensor (batch-wise or spatial) from local files, adapted for lattice-based quantum-aware processing.

    qa_encryption_analysis.m: Computes:

        NPCR (Number of Pixels Change Rate)

        UACI (Unified Average Changing Intensity)

        CCA (Correlation Coefficient Analysis) along horizontal, vertical, and diagonal directions, separately for RGB channels (3D plot)

        SSIM, PSNR for robustness analysis

        Pixel distribution plots for original vs. encrypted images (RGB histogram)

Output figures and metrics are saved in the results/ folder.
📌 Summary qa_encryption_analysis.m 
  qa_encryption_analysis.m includes:

    - Loop over 32 original and encrypted image pairs

    - Compute NPCR & UACI for each pair

    - Compute correlation coefficients per direction and channel

    - Generate histograms

    - Plot SSIM, PSNR scores

    - Save plots to results


