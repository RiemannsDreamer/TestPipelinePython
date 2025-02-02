# My Python Project

## Setup

### 1. Virtuelle Umgebung erstellen und aktivieren
```sh
python -m venv venv
source venv/bin/activate  # Windows: venv\Scripts\activate
```

### 2. Abhängigkeiten installieren
```sh
pip install -r requirements.txt
```

### 3. Tests ausführen
```sh
pytest --cov=app
```

### 4. Starten der Anwendung
```sh
python app.py
```

## CI/CD Pipeline
Die GitHub Actions Pipeline enthält:
- Linting mit `flake8`, `black`, `isort`
- Type Checking mit `mypy`
- Security Checks mit `bandit` und `safety`
- Unit-Tests mit `pytest` + Coverage-Report
- SonarCloud Code-Analyse
- Docker Build + Trivy Security Scan