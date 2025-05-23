# Relatório do Artigo - Predição de Desempenho Acadêmico com IA
## Artigo Escolhido
Título: Linear regression model to predict the use of artificial intelligence in experimental science students (adaptado metodologicamente para predição de desempenho escolar).
Autores: Elizeth Mayrene Flores Hinostroza, Derling Jose Mendoza, Mercedes Navarro Cejas, Edinson Patricio Palacios Trujillo.
Periódico: International Electronic Journal of Mathematics Education.
Ano de Publicação: 2025.
Fator de Impacto: Sim, indexado na Web of Science.
Descrição do Miniprojeto
Base de Dados Utilizada
Fonte: UCI Machine Learning Repository.
Link: https://doi.org/10.24432/C5TG7T
Descrição: Base composta por informações de desempenho acadêmico de estudantes do ensino médio em Portugal, nos cursos de Matemática e Português.

## Variáveis Selecionadas
G1: Nota no primeiro semestre.
G2: Nota no segundo semestre.
G3: Nota final (variável alvo).

## Tamanho da População
Total de Registros: 1044 estudantes (ambas as turmas de matemática e português combinadas).

## Divisão de Dados
Treinamento: 80%
Teste: 20%

## Validação Cruzada
Não foi aplicada validação cruzada, visto que foi utilizada uma divisão simples de treino e teste para fins de simplicidade.

## Algoritmo Utilizado
Regressão Linear Simples e Múltipla, onde G3 é prevista a partir de G1 e G2.

## Critérios de Hiperparâmetros
Não se aplica, pois regressão linear não depende de hiperparâmetros ajustáveis.

## Uso de Transfer Learning
Não utilizado.

## Técnicas de Regularização
Não aplicadas.

## Aumento de Dados
Não foi necessário, pois a base possui quantidade suficiente para uma regressão multipla e XGBoost Regression.

## Desbalanceamento de Classes
Não aplicável, pois é um problema de regressão.
Figuras de Mérito
Métricas Utilizadas:
- Desvio Padrão
- MAE (Erro Absoluto Médio)
- Média

# Implementação
Ambiente: Python (bibliotecas Pandas, Scikit-Learn e Matplotlib).
Processo:
1. Limpeza dos dados, considerando apenas as variáveis G1, G2 e G3.
2. Modelagem utilizando regressão linear.
3. Avaliação por meio das métricas descritas.
## Fontes de Implementação
- Documentação oficial do Scikit-Learn.
- Exemplos do Kaggle sobre análise da base Student Performance.
- UCI Machine Learning Repository.
## Modificações na Técnica
O artigo original aplica regressão para predição de uso de IA. No presente miniprojeto, o mesmo método foi adaptado para predição de nota final (G3) a partir das notas parciais G1 e G2.
## Contribuição dos Integrantes
Cada membro da equipe ficou responsável por:
- Coleta e entendimento dos dados;
- Pré-processamento e seleção de variáveis;
- Desenvolvimento e avaliação do modelo;
- Montagem do relatório e dos slides.
## Implementação do Miniprojeto
Ferramentas e Tecnologias Utilizadas
- Linguagem: Python
- Bibliotecas: pandas, scikit-learn, matplotlib, seaborn, rich

# Arquivos Utilizados
- Dados:
  - student-mat.csv
  - student-por.csv
- Código:
  - ai_topics.ipynb (Notebook com análise, modelagem e avaliação)
- Documentação:
  - README.md
  - requirements.txt

# Etapas da Implementação
1. Leitura e Preparação dos Dados:
   - Carregamento dos datasets student-mat.csv e student-por.csv.
   - Seleção das colunas G1, G2 e G3.
   - Junção dos dois datasets.

2. Análise Exploratória:
   - Estatísticas descritivas.
   - Análise de correlação entre G1, G2 e G3.
   - Visualização de dispersão e análise de outliers.

3. Criação do Modelo:
   - Definição de G1 e G2 como variáveis independentes e G3 como alvo.
   - Divisão dos dados em treino (80%) e teste (20%).
   - Treinamento do modelo de Regressão Linear Múltipla.

4. Avaliação do Modelo:
   - Cálculo das métricas: R², MAE, RMSE.
   - Plotagem da linha de regressão e análise dos resíduos.

5. Interpretação dos Resultados:
   - Avaliação dos coeficientes.
   - Discussão sobre os erros e possíveis melhorias.
