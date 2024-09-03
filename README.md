## Passo a passo do vídeo

### Getting started:
```bash
sudo apt install python3-venv
cd detect-test-pollution-main
python3 -m venv ./venv
source ./venv/bin/activate
pip install -r requirements.txt
```
### Testing
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

## Execução da Atividade

1. **Termo de Busca:**
   - `language:Python pytest in:readme created:>2020-01-01 size:<250`

2. **Repositório Escolhido:**
   - [https://github.com/mate-academy/py-knights-fighting](https://github.com/mate-academy/py-knights-fighting)

3. **Passos Realizados:**
   - Adicionadas as bibliotecas `pytest-cov` e `mutmut` ao `requirements.txt`.
   - Criado o ambiente virtual do projeto com `python3-venv` e instalação das dependências.
   - Criado um README principal adaptado aos passos do vídeo para este repositório.

4. **Resultados:**
   - **Cobertura:** Na primeira execução dos testes, verificou-se uma cobertura de 97% no arquivo principal.
     ![Screenshot from 2024-09-02 20-00-58](https://github.com/user-attachments/assets/08b5d2a9-a073-42d1-a972-45f8a85ff462)
     ![Screenshot from 2024-09-02 20-05-50](https://github.com/user-attachments/assets/2d149a2f-ccd4-4a7f-ab10-a6a26accf369)

   - **Mutação:** O primeiro relatório de mutação indicou 119 mutantes mortos e 227 mutantes sobreviventes, mostrando vulnerabilidades nos testes.
     
     ![Screenshot from 2024-09-02 20-05-33](https://github.com/user-attachments/assets/bde2f71f-ac80-422e-a2ea-28a54bcf2cfc)
     ![Screenshot from 2024-09-02 20-07-49](https://github.com/user-attachments/assets/a84aeda3-2def-451c-a7a2-472c505aaf9d)


5. **Após Alterações no Código:**
   - Redução dos mutantes sobreviventes para 189.
  ![Screenshot from 2024-09-02 22-12-07](https://github.com/user-attachments/assets/07ab82b9-9962-47f0-8017-39166273d770)


6. **Relatóriosl:**
   - [Relatório de Mutação Inicial](https://github.com/rodrigodesan/Teste_Software_Mutantes_2024_santana_rodrigo/blob/main/artefatos/mutants_report_initial.pdf)
   - [Relatório de mutação final](https://github.com/rodrigodesan/Teste_Software_Mutantes_2024_santana_rodrigo/blob/main/artefatos/mutants_report_final.pdf)
   - [Relatório de cobertura](https://github.com/rodrigodesan/Teste_Software_Mutantes_2024_santana_rodrigo/blob/main/artefatos/Coverage%20report.pdf)

