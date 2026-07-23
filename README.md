# Análise e Modelagem Preditiva de Popularidade de Filmes (TMDB)

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/gabrielamb2k/FundamentosIA/blob/main/notebook.ipynb)

Projeto prático desenvolvido para a disciplina de Inteligência Artificial, focado na aplicação de técnicas de Machine Learning para a predição da popularidade de filmes.
Projeto prático desenvolvido para a disciplina de Inteligência Artificial, focado na aplicação de técnicas de Machine Learning para a predição da popularidade de filmes.

## 🎯 Objetivo

Desenvolver uma aplicação de aprendizado de máquina capaz de prever a popularidade (`popularity`) de um filme utilizando como atributos preditivos o ano de lançamento (transformado em idade do filme), a nota média (`vote_average`) e a contagem de votos (`vote_count`) do conjunto de dados do TMDB.

## 👥 Integrantes

* Carlos Henrico Fontes Cabral
* Gabriel Almeida Mota Bomfim
* Pedro Caldas de Souze Lucas Marques

## 📊 Fonte dos Dados

* **Dataset:** [TMDB Top 10000 Movies Updated 2026](https://www.kaggle.com/datasets/siddharthbhakta/tmdb-top-10000-movies-updated-2026)[cite: 3]
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
