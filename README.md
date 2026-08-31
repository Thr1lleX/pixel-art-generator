# Pixel Art Generator 

A deep learning project trained **from scratch** to generate pixel art images from text prompts.


##  Overview

This project explores generative AI applied to pixel art:
- Train a model from scratch using **TensorFlow** and/or **PyTorch**
- Generate 8-bit / 16-bit style pixel art from text descriptions
- Experiment with architectures (GAN, Diffusion, VAE, Transformer...)

##  Project Structure

```
Pixel_art_generator/
├── data/
│   ├── raw/            # Original datasets (ignored by git)
│   └── processed/      # Pre-processed data (ignored by git)
├── src/
│   ├── data/           # Data loading & preprocessing
│   ├── models/         # Model architectures
│   ├── training/       # Training loops & utilities
│   └── inference/      # Generation / inference scripts
├── notebooks/          # Exploration & experiments (Jupyter)
├── configs/            # Hyperparameter config files (YAML/JSON)
├── outputs/            # Generated images & model checkpoints
├── tests/              # Unit tests
├── requirements.txt    # Python dependencies
└── README.md
```

##  Setup

### Prerequisites
- Python 3.10+
- Git

### Installation

```bash
# Clone the repository
git clone https://github.com/Thr1lleX/pixel-art-generator.git
cd pixel-art-generator

# Create and activate the virtual environment
python -m venv .venv

# On Windows
.venv\Scripts\activate

# On Linux/macOS
source .venv/bin/activate

# Install dependencies
pip install -r requirements.txt
```

##  Training

```bash
python src/training/train.py --config configs/default.yaml
```

##  Generate

```bash
python src/inference/generate.py --prompt "a tiny knight in pixel art style"
```
##  Experiments

Track training with TensorBoard:

```bash
tensorboard --logdir logs/
```

## Tech Stack

- **Deep Learning**: PyTorch / TensorFlow
- **Image Processing**: Pillow, NumPy
- **Experiment Tracking**: TensorBoard / WandB
- **Configuration**: Hydra / YAML

## 📄 License

MIT License – see [LICENSE](LICENSE) for details.
