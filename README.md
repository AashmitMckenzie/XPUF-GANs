# XPUF-GANs

# 🔐 XPUF-GANs: eXplainable GAN Architecture for PUF Data Generation

![License](https://img.shields.io/badge/license-MIT-blue.svg)
![Python](https://img.shields.io/badge/python-3.7%2B-blue)
![TensorFlow](https://img.shields.io/badge/TensorFlow-2.x-orange)

## 📌 Overview

**XPUF-GANs** is a novel architecture designed to generate robust, secure, and explainable Physical Unclonable Function (PUF) data using Generative Adversarial Networks (GANs). This project integrates explainability with deep generative models to ensure transparency and reliability in hardware security applications such as FPGA fingerprinting, anti-counterfeiting, and authentication systems.

## 🧠 Key Features

- 🚀 Custom GAN Architecture tailored for SRAM/Arbiter/RO-based PUF patterns.
- 🧩 Explainability Integration using SHAP & LIME to interpret model behavior.
- 🎯 High Fidelity Challenge-Response Pair (CRP) Generation using latent noise vectors.
- 🔍 Model Evaluation metrics including fidelity, uniqueness, and reliability.
- 📊 Visualization Tools for real-time PUF distribution and training curves.

## 🏗️ Architecture

The architecture comprises:

- Generator: Accepts latent noise + optional challenge vector, produces synthetic CRPs.
- Discriminator: Classifies real vs. fake PUF outputs.
- Explainability Block: Integrates SHAP/LIME to analyze influence of latent dimensions and CRP patterns.
- Training Engine: Optimized with Adam + LeakyReLU + BatchNorm for stable GAN convergence.


## ⚙️ Getting Started

### 1. Clone the Repository

```bash
git clone https://github.com/AashmitMckenzie/XPUF-GANs.git
cd XPUF-GANs
````

### 2. Install Dependencies

```bash
pip install -r requirements.txt
```

### 3. Run Training

```bash
python xpuf_gan.py --epochs 100 --latent_dim 128
```

### 4. Visualize Results

```bash
python evaluate.py
```

## 📊 Sample Results

* Generated vs Real CRPs
* Training Curves (Loss, Accuracy)
* SHAP/LIME Feature Attribution


## 📈 Evaluation Metrics

| Metric       | Description                               |
| ------------ | ----------------------------------------- |
| Uniqueness   | Measures distinctiveness between CRPs     |
| Reliability  | Measures response stability across trials |
| Uniformity   | Measures bit distribution randomness      |
| Bit Aliasing | Measures bias across all CRPs             |

## 🔬 Research Applications

* Secure ID Generation for IoT/Embedded Systems
* Clone Detection & Anti-Counterfeit Systems
* FPGA/ASIC Security Fingerprinting
* Adversarial PUF Analysis and Simulation

## 🙌 Contributions

We welcome contributions and suggestions! Feel free to:

* Report issues
* Improve model performance
* Add new evaluation metrics
* Integrate other explainability libraries

Please fork the repository and submit a pull request.

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## ⭐ Star This Repo

If you find this project helpful or inspiring, please consider ⭐ starring it on GitHub — it helps grow the community!

```
```
