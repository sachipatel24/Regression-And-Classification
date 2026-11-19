# Cars + Flowers: the dumb version

Same layout as the example you were given:

```
CarsAndFlowers/
  Regression_AutoMPG_Colab.ipynb       <- guess a car's MPG (number)
  Classification_Iris_Colab.ipynb      <- guess an iris type (group)
  docs/index.html                      <- the website (already written)
```

## Do this
1. Open each notebook in Google Colab and press Runtime -> Run all.
2. Each notebook downloads 2 files at the end:
   - Regression: `regression_model.onnx` and `regression_scaler.json`
   - Classification: `classification_model.onnx` and `classification_scaler.json`
3. Put those 4 files inside `docs/`, next to `index.html`.
4. Test on your laptop: open a terminal in `docs/` and run `python -m http.server 8000`, then go to http://localhost:8000
5. Make a public GitHub repo and upload everything.
6. Repo -> Settings -> Pages -> Deploy from a branch -> `main` -> `/docs` -> Save.
7. Your site is live at `https://YOUR-USERNAME.github.io/REPO-NAME/`.

Double-clicking `index.html` will NOT work (the browser blocks loading the model from a plain file). Use the local server or GitHub Pages.

## The 3 students per project
Small [16] (or [8]), Medium [64,32], Large [128,64,32]. The notebook prints a scoreboard and automatically exports the winner.
Scores: R2 (plus MAE, RMSE) for cars. Accuracy, Precision, Recall and F1 (plus confusion matrix and correlation matrix) for flowers.
