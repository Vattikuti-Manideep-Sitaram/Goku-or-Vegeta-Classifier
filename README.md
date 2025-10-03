# Goku or Vegeta Classifier

"Power comes in response to a need, not a desire." – Son Goku

Welcome, fellow Z Warrior! This repo is your training ground for building a computer vision model that can tell whether Earth's mightiest Saiyan on screen is Goku or Vegeta. Whether you are new to machine learning or just getting your feet wet after binge-watching Dragon Ball Z, this guide keeps things light-hearted, beginner friendly, and packed with references worthy of Capsule Corp.

## Saiyan Saga Overview
- **Mission**: Train a fastai neural network that distinguishes between images of Goku and Vegeta.
- **Why fastai?** Because transfer learning lets us skip straight to Super Saiyan without years in the Hyperbolic Time Chamber.
- **Who is this for?** Anime fans, Machine Learning Padawans, and anyone who has ever yelled "Kamehameha" at their computer.

## Project Layout (Map of the Saiyan Realm)
- `01_intro.ipynb` – The main notebook; walk through data gathering, model training, and evaluation.
- `goku_or_vegeta/` – Local image cache used in the notebook. Inside you will find `goku/` and `vegeta/` subfolders brimming with training images.
- `goku.jpg` / `vegeta.jpg` – Showcase images for quick sanity checks or memes.

## Power Level Requirements
- Python 3.9+ (any modern version works).
- Basic terminal powers (no Instant Transmission required).
- Packages:
  - `fastai`
  - `duckduckgo_search` (exposes `DDGS` for image scraping)
  - `fastdownload`
  - `jupyter`

Install everything the Capsule Corp way:
```bash
python -m venv venv
source venv/bin/activate  # On Windows use: venv\Scripts\activate
pip install fastai duckduckgo_search fastdownload jupyter
```
If you prefer conda:
```bash
conda create -n saiyan python=3.10
conda activate saiyan
pip install fastai duckduckgo_search fastdownload jupyter
```

## Training Arc (How to Use This Notebook)
1. Activate your virtual environment.
2. Launch Jupyter:
   ```bash
   jupyter notebook 01_intro.ipynb
   ```
3. Run the notebook cells top to bottom. Each cell includes comments that explain what is happening, so even Krillin can follow along.
4. When `learn.fine_tune(...)` begins, grab a senzu bean and watch the loss curves fall faster than Vegeta's pride after Kakarot goes Super Saiyan.

## Collecting More Ki (Extending the Dataset)
- The notebook already uses DuckDuckGo to grab images. You can re-run those cells to pull fresh shots.
- Drop any hand-curated images into `goku_or_vegeta/goku` or `goku_or_vegeta/vegeta` to enrich the dataset.
- Keep classes balanced; even Vegeta deserves an equal chance to shine.

## Model Techniques (Saiyan Science)
- **Transfer Learning**: Leverages a pretrained convolutional neural network, giving you ultra instinct-level accuracy with minimal data.
- **Data Augmentation**: fastai automatically performs flips, rotations, and more. Think of it as the Fusion Dance for images.
- **Evaluation**: Use the confusion matrix and interpretation tools at the end of the notebook to see who is getting mistaken for whom.

## Results to Expect
- With a balanced gallery of images, you can expect accuracy well above 90% after a few epochs.
- Review the misclassified images – sometimes Vegeta just looks suspiciously heroic.

## FAQ from King Kai
- **"I am new to deep learning. Is this too hard?"** Nope! The notebook is annotated and fastai manages the heavy lifting. Treat it like a guided training montage.
- **"Can I swap in other characters?"** Absolutely. Replace folders with other characters (Gohan vs. Trunks, Piccolo vs. Cell) and retrain.
- **"Do I need a GPU?"** A CPU will work for small runs, but a GPU (even a humble one) turns training time from Namek saga length to abridged episode length.

## Legendary Quotes to Keep You Motivated
- "There is no such thing as limits, only plateaus." – Vegeta (probably).
- "I do not fear this new challenge. Rather like a true warrior, I will rise to meet it." – Vegeta, hyping your hyperparameters.
- "You are better than this, Kakarot!" – Use this whenever your validation loss stalls.
- "It's not about strength; it's about being the best version of yourself." – Goku, encouraging good code hygiene.

## Contributing (Forming the Z Fighters)
1. Fork the repo, spin up your own branch like a Spiral Monday.
2. Push your improvements (new datasets, models, visualizations).
3. Open a pull request – friendly sparring welcome.

## License and Attribution
This project is for educational fun. Respect original artwork sources when expanding the dataset. Dragon Ball Z and its characters belong to Toei Animation, Shueisha, and Akira Toriyama. We are just fans pushing pixels and power levels.

Now go train that model. The fate of Earth (and your GitHub stars) depends on it.
