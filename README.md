# ☕ Checkpoint 01: Ciência de Dados - Impacto do Café no Sono

Este repositório contém o projeto prático de validação do Checkpoint Nível 1 da Alura, desenvolvido de forma totalmente isolada em ambiente local (`.venv`) para a empresa **Health&Life Analytics**. 

O objetivo estratégico do negócio é investigar o impacto estatístico, demográfico e comportamental do consumo diário de café e cafeína na arquitetura e quantidade de horas de sono de uma base histórica contendo 10.000 clientes globais.

---

## 🛠️ Infraestrutura e Ferramentas do Ambiente

* **Linguagem Base:** Python 3.12
* **Gerenciador de Dependências:** Virtual Env (`.venv`) isolado via Windows PowerShell
* **Bibliotecas de Manipulação de Dados:** Pandas, NumPy
* **Bibliotecas de Visualização Gráfica:** Matplotlib, Seaborn, Pillow
* **Machine Learning & Modelagem:** Scikit-Learn (Random Forest Classifier, Logistic Regression), Joblib

---

## 📊 Estrutura de Desenvolvimento do Notebook

O projeto foi totalmente fatiado e estruturado em células sequenciais individuais de Markdown e Código (Itens 1 ao 18), garantindo legibilidade e organização:

1. **Carga e Diagnóstico Estrutural (EDA):** Leitura dos dados brutos e auditoria completa de consistência de tipos, contagem de registros nulos e incidência de dados duplicados.
2. **Exploração de Variáveis Numéricas:** Construção de histogramas de distribuição e boxplots customizados (paleta salmão) para identificação de tendências centrais e caça a *outliers*.
3. **Exploração de Variáveis Categóricas:** Gráficos de pizza para proporção demográfica de gênero e barras horizontais em tons pastéis para volumetria dos Top 10 países.
4. **Análises Comparativas Avançadas:** Cruzamento tridimensional utilizando gráficos de dispersão (`scatterplot` com paleta magma) relacionando idade, estresse e consumo de café.
5. **Processamento Estatístico e Insights:** Extração dos impactos numéricos reais calculados diretamente das 10.000 linhas do dataset histórico.
6. **Machine Learning e Modelagem Preditiva:** Pipeline de classificação avaliando múltiplos algoritmos para prever a qualidade do sono (`Sleep_Quality`).
7. **Persistência de Arquivos:** Exportação física da base de dados limpa e salvamento do modelo campeão em formato binário.

---

## 🎯 Principais Conclusões de Negócio (Insights Reais)

* 📉 **O Fator Café:** Clientes posicionados na faixa de alto consumo de café (5 ou mais xícaras diárias) dormem em média **0.73 horas a menos** por noite (média de 6.14h) do que os clientes de baixo consumo (média de 6.88h).
* ⚡ **O Impacto do Estresse:** O nível de estresse provou ser a variable mais agressiva do ecossistema de saúde. Clientes com estresse classificado como **High** sofrem privação severa, registrando uma média de apenas **4.45 horas** de repouso por noite, enquanto o grupo **Low** alcança **7.24 horas**.
* 👥 **Simetria Demográfica:** As análises segmentadas comprovaram que a perda de sono provocada pela cafeína e pelo estresse comporta-se de forma simétrica entre homens, mulheres e demais grupos, indicando um padrão comportamental generalizado.

---

## 🤖 Desempenho dos Modelos Preditivos

* 🌲 **Random Forest Classifier (Modelo Campeão):** Alcançou **99.00% de acurácia** no conjunto de testes, apresentando métricas excelentes de precisão, recall e F1-Score em todas as classes avaliadas.
* 📈 **Regressão Logística:** Alcançou **78.85% de acurácia**, apresentando dificuldades pontuais (underfitting leve) para capturar as relações não-lineares complexas presentes na base.

---

## 💾 Arquivos Gerados no Pipeline (`/dados`)

* `synthetic_coffee_health_processed.csv`: Dataset final limpo, codificado (One-Hot Encoding) e contendo a feature derivada `Caffeine_per_Cup`.
* `melhor_modelo_random_forest.pkl`: Arquivo binário do modelo campeão exportado via `joblib` para deploy imediato em produção.

---

## 🚀 Como Executar o Projeto Localmente

1. Clone o repositório público:
   ```bash
   git clone git@github.com:Vagnerkrg/checkpoint-01.git
   ```
2. Instale as dependências contidas no arquivo de requerimentos:
   ```bash
   pip install -r requirements.txt
   ```
3. Abra o caderno `checkpoint_cafe_sono.ipynb` no VS Code e clique em **Run All**.
