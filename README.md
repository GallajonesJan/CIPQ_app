# CIPQ Implementation Tool — Flask App

**Creative Industry Policy Quadrant v2.0**  
Philippine Book Publishing Industry Analysis

## Setup & Run

```bash
pip install -r requirements.txt
python app.py
```

Then open: http://localhost:5050

## Features

- **Coding Workspace** — add, edit, delete narrative segments with full CIPQ metadata
- **Analytics Dashboard** — live CIPQ Index, domain scores, indicator rankings, priority flags, stakeholder & regional breakdowns
- **REST API** — `GET /api/indicators/<domain>` returns indicators as JSON

## Persistence

Data is currently held in memory. For production, replace the `entries` list in `app.py` with a SQLite or PostgreSQL database using Flask-SQLAlchemy.
