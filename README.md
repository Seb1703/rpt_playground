# RPT Playground

An interactive Jupyter environment for the RPT interview exercise, launchable in one click via [mybinder.org](https://mybinder.org), no local setup required.

## How to launch

1. Go to [mybinder.org](https://mybinder.org).
2. Paste the URL of this repository into the **"GitHub repository name or URL"** field.
3. Click **"launch"** and wait ~1 minute while the environment builds.
4. A Jupyter session opens in your browser with all required Python packages pre-installed.

## Setting up the RPT token

1. In JupyterLab, open a terminal: **File → New → Terminal**
2. Run:
```bash
cp config.example.json config.json
```
3. Right-click `config.json` in the file browser → **Open With → Editor**, replace `YOUR_TOKEN_HERE` with the RPT token you received, and save (Ctrl+S / Cmd+S).

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
| `config.example.json` | Template for `config.json` |
