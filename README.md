# Desafio Cientista de Dados - Análise de Filmes (Indicium)

Este repositório contém a resolução do desafio técnico para a vaga de Cientista de Dados, focada na análise de um dataset de filmes do IMDB e na construção de um modelo preditivo para orientar as decisões de negócio de um estúdio de Hollywood.

## Estrutura do Projeto

- `data/desafio_indicium_imdb.csv`: O dataset original utilizado na análise.
- `notebooks/analise_filmes.ipynb`: Jupyter Notebook com toda a análise exploratória, tratamento dos dados, respostas às perguntas e o código de modelagem.
- `modelo_imdb_prediction.pkl`: O modelo de Machine Learning (`RandomForestRegressor`) treinado e salvo.
- `requirements.txt`: Arquivo com as dependências Python para reproduzir o ambiente de execução.

## Como Executar

1.  Clone este repositório para a sua máquina local.
2.  Navegue até a pasta raiz do projeto.
3.  Crie e ative um ambiente virtual:
    ```bash
    # Criar ambiente
    python -m venv venv
    # Ativar no Windows
    .\venv\Scripts\activate
    # Ativar no macOS/Linux
    source venv/bin/activate
    ```
4.  Instale as dependências necessárias:
    ```bash
    pip install -r requirements.txt
    ```
5.  Abra o Jupyter Notebook `notebooks/analise_filmes.ipynb` para visualizar e executar a análise completa.

## Resumo dos Resultados

* **Análise Exploratória:** A análise identificou que a popularidade de um filme (medida pelo `No_of_Votes`) e o gênero são os principais fatores correlacionados com um alto faturamento. Gêneros de apelo massivo como Aventura, Animação e Ação mostraram ser os mais lucrativos em média.
* **Modelo Preditivo:** Foi desenvolvido um modelo `RandomForestRegressor` para prever a nota do IMDB. O modelo obteve um **RMSE de aproximadamente 0.26** no conjunto de teste e previu uma **nota de 8.75** para o filme de exemplo, demonstrando boa acurácia.
