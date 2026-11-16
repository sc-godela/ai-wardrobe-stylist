# 👕 AI Wardrobe Stylist
Recommends menswear outfits using deep learning, trained on outfits
made by professional ASOS stylists.

## How it works
1. **CLIP** turns each clothing photo into numbers (an embedding)
2. A **neural network** learns which items go well together
3. A **web app** suggests outfits from your own clothes

## Dataset
**[ASOS Outfits](https://osf.io/cg6eq/?view_only=f446b0f51bca409da4175a4ce8d9000a)**,
272k menswear outfits made by ASOS stylists
([paper](https://arxiv.org/abs/1904.00741)).

*Why not [Polyvore](https://github.com/xthan/polyvore-dataset)?*
It's almost entirely womenswear (48 vs 1 gendered titles in a
2,000-item sample, see `notebooks/01_explore_dataset.ipynb`).

> ⚠️ ASOS image links currently return HTTP 503, under investigation.

## Progress
- [x] Project setup
- [x] Dataset exploration → chose ASOS menswear
- [ ] 🔄 Get ASOS images
- [ ] Generate CLIP embeddings
- [ ] Train compatibility model
- [ ] Evaluate (AUC, fill-in-the-blank)
- [ ] Web app + deploy

## Tech
Python · pandas · PyTorch · CLIP · Google Colab · Gradio · Hugging Face
