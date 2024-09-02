## Passo a passo do vídeo

## Installation or Getting Started

Getting started:
```bash
sudo apt install python3-venv
cd detect-test-pollution-main
python3 -m venv ./venv
source ./venv/bin/activate
pip install -r requirements.txt
```
## Testing
```bash
# run tests normally
pytest -vv

#perform tests with line (node) coverage report
pytest -vv --cov
# perform tests with branch coverage report
pytest -vv  --cov  --cov-branch  --cov-report html

#run tests with mutmut
mutmut run --paths-to-mutate= .. /py-knights-fighting/app/main.py

mutmut results
mutmut show [id]

# Gerar relatório de mutação
mutmut html
```
