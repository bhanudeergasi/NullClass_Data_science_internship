
Each folder contains:
- `*.ipynb`: Jupyter notebook with full implementation.
- `requirements.txt`: Required dependencies.
- (Optional) Drive link to large models.

---

##  Tasks Overview

### **Task 1: Text Tokenization & Encoding using Pretrained BERT**
-  Used Hugging Face’s BERT for tokenization and encoding.
-  Cleaned and balanced the IMDB dataset.
-  Trained a binary classification model.
-  Model saved and linked via Google Drive (see below).

 **[Model Link (Task 1)](https://drive.google.com/file/d/1-4a6UqWX39oYnlWkLAFNd12y5dmxnmxN/view?usp=drive_link)**

---

### **Task 2: Conditional GAN for Simple Shape Generation**
-  Conditional GAN (CGAN) trained to generate basic shapes (e.g., squares, circles).
-  Used PyTorch to build generator/discriminator.
-  Labels conditioned on generator input.
-  GAN loss monitored and visualized.

---

### **Task 3: Text Embedding using CLIP**
-  Tokenized and embedded prompts using OpenAI’s CLIP model.
-  Saved vector embeddings to `.pt` file.
-  Calculated CLIP scores between generated dummy images and prompts.

---

### **Task 4: Complete Text-to-Image Pipeline (GAN + Stable Diffusion)**
-  Combined:
  - Text preprocessing
  - Text embedding (CLIP)
  - Image generation
-  GAN-based generation showed poor image quality.
-  Switched to **Stable Diffusion** for high-quality outputs.
-  Pipeline demonstrates real-world integration.

 `generated_images/` (are also submitted in TASK4 folder)

---

### **Task 5: Fine-Tuning Stable Diffusion for Artwork**
-  Domain: **Artwork generation**
-  Used LoRA (Low-Rank Adaptation) to fine-tune on 10 custom artwork-caption pairs.
-  Generated new artwork using trained model.
-  Due to hardware limits, small batch + epochs used for training stability.
-  Model saved and linked via Google Drive (see below).

 **[Model Link (Task 5)](https://drive.google.com/file/d/1cLIW0fn8R93_4O2ZQMnWXRyZH_up8MX4/view?usp=drive_link)**


---

##  Environment

All tasks were developed using:

- Python 3.11+
- Google Colab + T4 GPU
- Hugging Face Transformers & Diffusers
- Torchvision, PIL, NumPy, Matplotlib

---

##  Instructions to Run

```bash
# Example for Task 1
cd task1_tokenization_encoding/
pip install -r requirements.txt
# Open the notebook and run cells
