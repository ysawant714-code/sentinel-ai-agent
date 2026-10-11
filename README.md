# Sentinel AI — Single Agent Project

## What it does
- Takes example security activity values.
- Uses a Random Forest ML model trained on synthetic demo data.
- A single agent selects LOW, MEDIUM, or HIGH risk and an action.
- Shows results in a Streamlit dashboard.

**Safety and limitations:** It does not monitor a real network or block real IP addresses. Blocking is simulated. The initial model uses synthetic data for learning/demo purposes; its metrics are not real-world security claims.

## Run on Windows
1. Install Python 3.11 or 3.12 from https://www.python.org/downloads/ and tick **Add Python to PATH**.
2. Extract this ZIP.
3. Open the extracted folder in File Explorer. Click the address bar, type `cmd`, and press Enter.
4. Run these commands one by one:

```bash
py -m venv .venv
.venv\\Scripts\\activate
py -m pip install --upgrade pip
pip install -r requirements.txt
streamlit run app.py
```

5. A browser tab opens. If not, open `http://localhost:8501`.
6. Stop with Ctrl+C in the terminal.

If `py` is not recognized, try `python --version`. If neither works, reinstall Python and enable Add Python to PATH.

## Files
- `app.py`: dashboard, demo model, and single-agent decision policy.
- `requirements.txt`: Python libraries.
- `README.md`: setup instructions.
