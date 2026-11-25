# CyberSentinel: AI-Powered Digital Trust & Cyber Defence Platform

**CyberSentinel** is a real-time threat detection, unmasking, and active cyber defence platform built with **Flask**, **PostgreSQL**, and **React (Vite)**.

## Architecture & Tech Stack
- **Backend:** Python, Flask, Flask-CORS, Psycopg2 (`app.py`, `detector.py`, `database.py`)
- **Database:** PostgreSQL (`JSONB` threat indicator storage & historical analytics)
- **Frontend:** React 18, Vite (`src/App.jsx`, `src/components/`)

## API Endpoints
- `POST /api/analyze` — Analyzes a URL or message, calculates risk score & severity, and stores evidence in PostgreSQL.
- `GET /api/alerts` — Fetches recent threat detections for the live alert feed.
- `GET /api/stats` — Returns total scans, phishing counts, critical alerts, average risk score, and 7-day breakdown.

## Local Setup & Run Instructions

### 1. Create PostgreSQL Database
```bash
createdb -U postgres cybersentinel
