# RPT Playground

An interactive Jupyter environment for the RPT interview exercise, launchable in one click via [mybinder.org](https://mybinder.org), no local setup required.

## How to launch

1. Go to [mybinder.org](https://mybinder.org).
2. Paste the URL of this repository into the **"GitHub repository name or URL"** field.
3. Click **"launch"** and wait ~1 minute while the environment builds.
4. A Jupyter session opens in your browser with all required Python packages pre-installed.

## First steps after launch

1. In the file browser on the left, create a new file named **`config.json`** in the root directory.
2. Add your RPT Playground token:

```json
{
  "RPT_TOKEN": "YOUR_TOKEN_HERE",
  "RPT_API_URL": "https://rpt.cloud.sap/api/predict"
}
```

3. Open **`playground.ipynb`** and start the exercise.


## What's included

| File | Description |
|---|---|
| `playground.ipynb` | Interview notebook |
| `employee_salaries.csv` | Dataset for the exercise |
| `requirements.txt` | Python dependencies (installed automatically by Binder) |
| `config.example.json` | Template for `config.json` |
