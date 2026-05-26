# Pipeline de PLN para análise de avaliações de e-commerce

**Aluno:** Breno dos Santos Mota  
**Professor:** Fernando Guimarães Ferreira  
**Disciplina:** Processamento de Linguagem Natural  
**Corpus:** RePro — avaliações de produtos em português  
**Problema analítico:** identificar sentimentos, temas recorrentes, padrões de reclamação e relações entre produtos, categorias, marcas e tópicos.

## Objetivo do projeto

Construir um pipeline completo de Processamento de Linguagem Natural para transformar avaliações textuais brutas em informações úteis, combinando pré-processamento textual, representação vetorial, busca textual, classificação, modelagem de tópicos, extração de entidades, grafo de conhecimento e visualizações interpretáveis.

## Mapa da rubrica no notebook

| Parte do enunciado | Seção no notebook |
|---|---|
| 0. Setup do ambiente e coleta do corpus | Seção 0 |
| 1. Pré-processamento textual com NLTK e spaCy | Seção 1 |
| 2. Representação vetorial e busca textual | Seção 2 |
| 3. Modelagem, classificação ou análise de sentimento | Seção 3 |
| 4. NER, extração de informação e grafo de conhecimento | Seção 4 |
| 5. Visualização, comunicação e reprodutibilidade | Seção 5 |

## Estrutura do projeto

- `data/raw/`: dados brutos.
- `data/interim/`: dados intermediários.
- `data/processed/`: dados processados.
- `notebooks/`: notebooks do projeto.
- `outputs/figures/`: figuras geradas.
- `outputs/tables/`: tabelas geradas.
- `outputs/models/`: modelos salvos.
- `outputs/graphs/`: grafos exportados.
- `reports/`: relatório final em PDF.

## Como executar

1. Abra o Anaconda Prompt na pasta do projeto.

2. Crie o ambiente Conda, apenas na primeira execução:

   `conda create -n pln-repro python=3.11 -y`

3. Ative o ambiente Conda:

   `conda activate pln-repro`

4. Atualize o pip:

   `python -m pip install --upgrade pip`

5. Instale as dependências do projeto:

   `pip install -r requirements.txt`

6. Baixe o modelo de português do spaCy:

   `python -m spacy download pt_core_news_sm`

7. Registre o ambiente como kernel do Jupyter, caso necessário:

   `python -m ipykernel install --user --name pln-repro --display-name "Python (pln-repro)"`

8. Abra o JupyterLab:

   `jupyter lab`

9. No JupyterLab, abra o notebook principal:

   `main_end_to_end_pln.ipynb`

10. Selecione o kernel `Python (pln-repro)` e execute as células em ordem.