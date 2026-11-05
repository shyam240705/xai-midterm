# LayerCAM vs. Transformer Attribution (XAI Midterm)

Shyam Patel - Deep Learning Midterm Project, Topic 1 - Fall 2026

Compares explanation heatmaps from a pretrained ResNet-50 (LayerCAM, last block `layer4[-1]`)
and a pretrained ViT-B/16 (Chefer et al. Transformer Attribution) on four images.

## Contents
- `Shyam_Patel_XAI_Midterm_Report_Final.docx` / `.pdf` - report
- `Shyam_midterm_multi_image.ipynb` - code (Google Colab)
- `results/` - comparison figures, overlays, and `prediction_results.csv`

## How to run
1. Open the notebook in Google Colab and select a GPU runtime (Runtime > Change runtime type > T4 GPU).
2. Run all cells in order. The first cell installs `grad-cam` and `timm` and clones
   https://github.com/hila-chefer/Transformer-Explainability.
3. When prompted in section 6, upload three JPG/PNG images. Figures and the CSV are saved to
   `/content/xai_results/multi_image/` and downloaded as a ZIP.

Note: ResNet-50 uses ImageNet normalization; the ViT uses mean = std = 0.5 per channel.
