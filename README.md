# 🏠 House Prices Prediction — Kaggle Project

## 📌 Visão Geral

Este projeto tem como objetivo prever o preço de venda de casas (**SalePrice**) utilizando técnicas de **Machine Learning**, com base no famoso dataset **House Prices: Advanced Regression Techniques** do Kaggle.

O foco principal foi desenvolver um **pipeline completo**, desde a análise exploratória dos dados (EDA) até a submissão final no Kaggle, aplicando boas práticas de ciência de dados e engenharia de atributos.

---

## 🎯 Objetivo

Construir um modelo de regressão capaz de prever o preço de imóveis residenciais com alta precisão, utilizando:

* Feature Engineering
* Pipelines do scikit-learn
* Transformações de target
* Avaliação por métrica oficial do Kaggle (RMSE)

---

## 📂 Estrutura do Projeto

```
├── notebooks/
│   ├── 01_exploracao_dados.ipynb
│   └── 02_eda_aprofundada.ipynb
│
├── data/
│   ├── train.csv
│   └── test.csv
│
├── README.md
└── .gitignore
```

---

## 🔍 Etapas do Projeto

### 1️⃣ Análise Exploratória de Dados (EDA)

* Avaliação de distribuições
* Identificação de outliers
* Análise de correlação com `SalePrice`
* Entendimento das variáveis numéricas e categóricas

### 2️⃣ Feature Engineering

Foram criadas novas variáveis para capturar melhor o contexto temporal e estrutural dos imóveis:

* **HouseAge** → Idade do imóvel
* **RemodAge** → Anos desde a última reforma
* **TotalHouseArea** → Área total construída

Essas features melhoraram significativamente o desempenho do modelo.

### 3️⃣ Pré-processamento

* Separação de `X` e `y`
* Transformação do target usando `log1p`
* Tratamento de valores ausentes com `SimpleImputer`
* Uso de `ColumnTransformer` para organização do pipeline

### 4️⃣ Modelagem

* Modelo utilizado: **Linear Regression**
* Implementação via `Pipeline` do scikit-learn
* Evita vazamento de dados e garante reprodutibilidade

### 5️⃣ Avaliação

* Métrica: **RMSE (Root Mean Squared Error)**
* Avaliação em treino e validação
* Predições finais revertidas com `expm1`

---

## 🏆 Resultado Final

📊 **Score Kaggle:** `0.13771`

Esse resultado posiciona o projeto em um nível **competitivo**, acima do esperado para projetos introdutórios, demonstrando:

* Bom domínio de pipeline
* Feature engineering eficaz
* Estrutura profissional de ML

---

## 🧠 Tecnologias Utilizadas

* Python 3.11
* Pandas
* NumPy
* Scikit-learn
* Jupyter Not

---

📬 *Projeto desenvolvido para fins educacionais e de portfólio.*
