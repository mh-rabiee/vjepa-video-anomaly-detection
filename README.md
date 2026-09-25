# V-JEPA Video Anomaly Detection

Video anomaly detection on the UCF-Crime dataset using a frozen **V-JEPA** encoder
for feature extraction and a **k-NN novelty detector** trained only on normal
footage.

🚧 **Ongoing research project** — part of ongoing work at the **AISL Lab**. Pipeline
and results are still evolving.

## Pipeline
`Normal videos → V-JEPA (ViT-L/16) embeddings → KNN novelty detector → anomaly score`

## Status
- [x] V-JEPA feature extraction pipeline
- [x] Baseline KNN anomaly detector
- [ ] Full test-set evaluation

## Future Work
- Improve the anomaly classifier/detector (beyond simple k-NN)
- Experiment with alternative backbones
- Train/evaluate on the complete dataset

## Run it
Open `VJEPA_VAD_organized.ipynb` in Google Colab (GPU runtime). Requires a Kaggle
API token for dataset download — see notebook for details.

## Acknowledgments
[V-JEPA](https://github.com/facebookresearch/jepa) (Meta AI) · UCF-Crime dataset

