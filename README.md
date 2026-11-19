# Cars + Flowers

## Project Files

```text
CarsAndFlowers/
├── Regression_AutoMPG_Colab.ipynb
├── Classification_Iris_Colab.ipynb
└── docs/
    └── index.html
```

## Steps

1. Open both notebooks in Google Colab.
2. Click **Runtime → Run all**.
3. Download the two files from each notebook:
   - Regression: `regression_model.onnx` and `regression_scaler.json`
   - Classification: `classification_model.onnx` and `classification_scaler.json`
4. Put all four files inside the `docs/` folder.
5. Upload the project to a public GitHub repository.
6. Go to **Settings → Pages**.
7. Select **Deploy from a branch**, choose `main` and `/docs`, then click **Save**.

Your website will be available through GitHub Pages.

## Models

Each notebook compares three models:

- Small: `[16]`
- Medium: `[64, 32]`
- Large: `[128, 64, 32]`

The regression notebook predicts car MPG.

The classification notebook predicts the iris flower type.
