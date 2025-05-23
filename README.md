
# Relatório do Artigo - Predição de Desempenho Acadêmico com IA

## Artigo Escolhido

- **Título:** *Linear regression model to predict the use of artificial intelligence in experimental science students* (adaptado metodologicamente para predição de desempenho escolar).
- **Autores:** Elizeth Mayrene Flores Hinostroza, Derling Jose Mendoza, Mercedes Navarro Cejas, Edinson Patricio Palacios Trujillo.
- **Periódico:** International Electronic Journal of Mathematics Education.
- **Ano de Publicação:** 2025.
- **Fator de Impacto:** Sim, indexado na Web of Science.

## Descrição do Miniprojeto

### Base de Dados Utilizada
- **Fonte:** UCI Machine Learning Repository.
- **Link:** https://doi.org/10.24432/C5TG7T
- **Descrição:** Dados acadêmicos de alunos do ensino médio em Portugal, dos cursos de Matemática e Português.

### Variáveis Selecionadas
- **G1:** Nota no primeiro semestre.
- **G2:** Nota no segundo semestre.
- **G3:** Nota final (variável alvo).

### Tamanho da População
- **Total:** 1044 registros (junção dos datasets de matemática e português).

### Divisão de Dados
- **Treinamento:** 80%
- **Teste:** 20%

### Validação Cruzada
- Não foi utilizada validação cruzada, apenas divisão simples de treino e teste.

### Algoritmos Utilizados
- **Regressão Linear Múltipla:** Modelo base, simples e interpretável.
- **XGBoost Regressor:** Algoritmo de boosting que melhora a capacidade preditiva.

### Critérios de Hiperparâmetros
- **Regressão Linear:** Não aplicável.
- **XGBoost:** Teste manual dos hiperparâmetros `n_estimators`, `max_depth` e `learning_rate`.

### Uso de Transfer Learning
- Não utilizado.

### Técnicas de Regularização
- **XGBoost:** Regularização L1 e L2 intrínseca.
- **Regressão Linear:** Não aplicada.

### Aumento de Dados
- Não necessário.

### Desbalanceamento de Classes
- Não aplicável (problema de regressão).

## Figuras de Mérito

- **R²** — Coeficiente de Determinação.
- **MAE** — Erro Absoluto Médio.
- **RMSE** — Raiz do Erro Quadrático Médio.
- **Desvio Padrão dos Erros.**
- **MEAN**

## Implementação do Miniprojeto

### Ferramentas e Tecnologias
- **Linguagem:** Python
- **Bibliotecas:** pandas, scikit-learn, xgboost, matplotlib, seaborn, rich

### Arquivos do Projeto
- **Dados:** student-mat.csv, student-por.csv
- **Código:** Notebook.ipynb
- **Documentação:** README.md, requirements.txt

### Etapas da Implementação
1. **Leitura e Preparação dos Dados**
2. **Análise Exploratória**
3. **Criação dos Modelos**
4. **Avaliação dos Modelos**
5. **Interpretação dos Resultados**

## Fontes e Referências
- Documentação do Scikit-Learn
- Documentação do XGBoost
- Kaggle - Student Performance Dataset
- UCI Machine Learning Repository
- Código: Notebook.ipynb

## Modificações na Técnica
- Adaptação do artigo original para predição de **nota final (G3)** com base em **G1** e **G2**.
- Inclusão de modelo avançado XGBoost além da regressão linear.

## Contribuição dos Integrantes
- Coleta e compreensão dos dados. (Russo e Maiara)
- Análise exploratória e pré-processamento. (Maiara)
- Desenvolvimento e comparação dos modelos. (Russo)
- Geração de visualizações, relatório e documentação. (Russo)
- Preparação dos slides e apresentação. (Maiara)
