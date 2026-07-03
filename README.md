# ☕ Checkpoint 01 — Coffee Consumption & Sleep Impact Analysis

Projeto de Data Science aplicado à análise do impacto do consumo de cafeína na qualidade do sono, utilizando técnicas de EDA, estatística descritiva e Machine Learning.

Base de dados com **10.000 registros** simulando comportamento de clientes globais.

---

## 🎯 Objetivo

Investigar como o consumo diário de café, nível de estresse e variáveis demográficas influenciam diretamente a duração e qualidade do sono, gerando insights estatísticos e modelos preditivos.

---

## 🛠️ Stack Utilizada

- Python 3.12  
- Pandas | NumPy  
- Matplotlib | Seaborn | Pillow  
- Scikit-Learn (Random Forest, Logistic Regression)  
- Joblib  
- Ambiente virtual (.venv)

---

## 📊 Pipeline do Projeto

### 1. EDA e Qualidade dos Dados
- Verificação de nulos, duplicados e consistência de tipos
- Análise de distribuições (histogramas e boxplots)
- Identificação de outliers

### 2. Análise Exploratória
- Relação entre consumo de café e horas de sono
- Segmentação por gênero e faixa etária
- Impacto do nível de estresse no sono

### 3. Insights Estatísticos
- Diferença média de sono entre alto e baixo consumo de cafeína
- Correlação entre estresse e privação de sono
- Padrões demográficos consistentes entre grupos

---

## 🤖 Modelagem Preditiva

### Random Forest Classifier (Modelo Principal)
- Acurácia: **99%**
- Melhor desempenho geral entre os modelos testados

### Regressão Logística
- Acurácia: **78.85%**
- Menor capacidade de captura de relações não-lineares

---

## 📈 Principais Insights

- ☕ Alto consumo de cafeína reduz em média ~0.7h de sono por noite  
- ⚡ Estresse alto é o principal fator de privação de sono  
- 👥 Efeito consistente entre diferentes perfis demográficos  

---

## 💾 Artefatos Gerados

- `synthetic_coffee_health_processed.csv`
- `melhor_modelo_random_forest.pkl`

---

## 🚀 Execução Local

```bash
git clone git@github.com:Vagnerkrg/checkpoint-01.git
cd checkpoint-01
pip install -r requirements.txt
jupyter notebook
