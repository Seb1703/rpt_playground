# RPT Playground

An interactive Jupyter environment for the RPT interview exercise, launchable in one click via Google Colab, no local setup required.

## How to launch (recommended — Google Colab)

1. Open **[playground.ipynb in Colab](https://colab.research.google.com/github/Seb1703/rpt_playground/blob/HEAD/playground.ipynb)**.
2. In the **Setup** cell, replace `PASTE_YOUR_TOKEN_HERE` with the RPT token you received.
3. Run the **Setup** and **Load Data** cells — the notebook downloads the dataset automatically.

Colab already has all required packages pre-installed, and the notebook fetches its own data file, so there is nothing else to set up.

## Alternative — mybinder.org (backup)

1. Go to [mybinder.org](https://mybinder.org), paste **`https://github.com/Seb1703/rpt_playground`**, and click **launch** (~1 min build).
2. Open `playground.ipynb`, replace `PASTE_YOUR_TOKEN_HERE` in the Setup cell with your token, and run the cells.

The token is set directly in the notebook — same flow as Colab, no config file needed.

## Sharing the session (pair programming)

To share your running session with an interviewer:

1. Open a terminal: **File → New → Terminal**
2. Run:
```bash
echo "https://hub.2i2c.mybinder.org${JUPYTERHUB_SERVICE_PREFIX}lab?token=$(jupyter server list 2>/dev/null | grep -oP '(?<=token=)[^ ]+')"
```
3. Send the printed URL to your interviewer — they can open it directly in their browser to join the same session.

## What's included

| File | Description |
|---|---|
| `playground.ipynb` | Interview notebook |
| `api_reference.ipynb` | Full API documentation |
| `employee_salaries.csv` | Dataset for the exercise |
| `requirements.txt` | Python dependencies (installed automatically by Binder) |
