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
	pytest -vv  test_cal.py

	#perform tests with line (node) coverage report
	pytest -vv  test_cal.py  --cov=cal

	# perform tests with branch coverage report
	pytest -vv  test_cal.py  --cov=cal  --cov-branch  --cov-report html

	#run tests with mutmut
	mutmut run --paths-to-mutate= .. /detect-test-pollution-main/cal.py

	mutmut results
	mutmut show [id]

  # Gerar relatório de mutação
	mutmut html
```
