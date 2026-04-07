# Explainable AI for Chest X-ray Classification

This project compares **Grad-CAM** and **SHAP** for explaining a CNN model that classifies chest X-ray images.

## Project goal
The aim is to study how explainability methods can help interpret model predictions in a medical imaging task.

## Dataset
Use the **Chest X-ray Pneumonia** dataset from Kaggle, or a similar chest X-ray dataset.

Expected folder structure:

```text
dataset/
    train/
        NORMAL/
        PNEUMONIA/
    val/
        NORMAL/
        PNEUMONIA/
    test/
        NORMAL/
        PNEUMONIA/
```

## Files
- `xai_chest_xray.ipynb` – main notebook
- `requirements.txt` – required libraries
- `README.md` – project instructions

## Methods used
- **ResNet50** with transfer learning for image classification
- **Grad-CAM** for visual heatmap explanations
- **SHAP** for feature attribution explanations

## How to run
1. Download the dataset from Kaggle.
2. Arrange the dataset using the folder structure above.
3. Install dependencies:

```bash
pip install -r requirements.txt
```

4. Open the notebook:

```bash
jupyter notebook xai_chest_xray.ipynb
```

5. Run all cells.

## Outputs
The notebook:
- loads and preprocesses chest X-ray images
- trains a CNN model
- evaluates model performance with classification metrics
- generates Grad-CAM heatmaps
- generates SHAP explanations

## Notes
- SHAP can take longer to run because image explanations are computationally expensive.
- You may need to reduce the background sample size if your machine is slow.
- Update the dataset path in the notebook before running it.

## Report citation example
You can cite the code in your report like this:

> The implementation code for this project is available in the accompanying GitHub repository.

