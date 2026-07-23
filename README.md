# Análise e Modelagem Preditiva de Popularidade de Filmes (TMDB)

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/gabrielamb2k/FundamentosIA/blob/main/notebook.ipynb)

Projeto prático desenvolvido para a disciplina de Inteligência Artificial, focado na aplicação de técnicas de Machine Learning para a predição da popularidade de filmes.

---

## 🎯 Objetivo

Desenvolver uma aplicação de aprendizado de máquina capaz de prever a popularidade (`popularity`) de um filme utilizando como atributos preditivos o ano de lançamento (transformado em idade do filme), a nota média (`vote_average`) e a contagem de votos (`vote_count`) do conjunto de dados do TMDB.

## 👥 Integrantes

* Carlos Henrico Fontes Cabral
* Gabriel Almeida Mota Bomfim
* Pedro Caldas de Souze Lucas Marques

## 📊 Fonte dos Dados

* **Dataset:** [TMDB Top 10000 Movies Updated 2026](https://www.kaggle.com/datasets/siddharthbhakta/tmdb-top-10000-movies-updated-2026)
* **Plataforma:** Kaggle

## 🧠 Tipo da Tarefa

O problema foi tratado como uma tarefa de Aprendizado Supervisionado do tipo **Regressão**, tendo como atributo-alvo uma variável numérica contínua, a `popularity` dos filmes.

## 📁 Organização dos Arquivos

```text
FundamentosIA/
│
├── notebook.ipynb         # Arquivo principal com o código, treinamentos e análises
├── README.md              # Documentação principal do projeto
└── moviesTMBD.csv         # Base de dados utilizada no treinamento

🚀 Instruções para abrir no Google Colab
O botão azul Open in Colab no topo deste arquivo permite que você abra o código na nuvem sem precisar instalar nada no seu computador. Para executar o projeto:

Clique no botão azul "Open in Colab" no topo da página.

Você será redirecionado para o ambiente do Google Colab.

Execute as células em ordem para reproduzir as análises, o pré-processamento e as predições.

🤖 Modelos Utilizados
Foi feita a aplicação de algoritmos preditivos numéricos, com foco primário em:

Regressão Linear: Utilizado para prever a relação entre os dados transformados logaritmicamente (como vote_count e popularity).

Decision Tree Regressor (Árvore de Decisão): Avaliado para tentar captar padrões de decisão em cascata dos engajamentos.

Random Forest Regressor: Aplicado como modelo preditivo robusto para capturar padrões complexos.

📈 Principais Resultados
Impacto das Variáveis: Ao processar a Regressão Linear utilizando os dados com transformação logarítmica para atenuar outliers, os coeficientes demonstraram que a quantidade de votos e a média das notas têm um peso consideravelmente maior na popularidade do que a idade do filme.

Métricas do Modelo Inicial: O modelo de Regressão Linear obteve um R² de aproximadamente 0.48, explicando parte significativa da variação com apenas três variáveis preditoras, e a análise gráfica dos resíduos não apontou grandes vieses sistemáticos visuais.

Melhor Desempenho: No comparativo geral com os outros algoritmos implementados no notebook, o modelo Random Forest obteve as melhores métricas finais.

👨‍💻 Divisão das Contribuições
O projeto foi desenvolvido de forma colaborativa, com a seguinte divisão de foco:

Gabriel Almeida Mota Bomfim: Implementação do código-fonte em Python, preparação dos dados e treinamento dos modelos de Machine Learning (Regressão Linear, Árvore de Decisão e Random Forest).

Pedro Caldas de Souza Lucas Marques: Extração e consolidação das métricas de avaliação (MAE, MSE, RMSE, R²) e geração dos gráficos de análise de resíduos dos modelos.

Carlos Henrico Fontes Cabral: Revisão metodológica, adequação do código para execução em nuvem (Google Colab), redação das justificativas teóricas, interpretação analítica dos resultados e organização geral da documentação no GitHub.
