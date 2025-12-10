# Análise de Estatísticas de Jogadores da NBA

## Descrição do Projeto

Este projeto realiza uma análise completa de estatísticas de jogadores da NBA utilizando técnicas de Análise Exploratória de Dados (EDA) e Machine Learning. O objetivo é predizer a performance ofensiva dos jogadores através de duas abordagens: regressão (pontos por jogo) e classificação (identificação de high scorers).

### Objetivos

- **Regressão**: Predizer pontos por jogo usando características físicas, métricas de eficiência e contexto de carreira
- **Classificação**: Identificar jogadores com alto potencial ofensivo (>15 ppg)
- **Comparação de algoritmos**: Avaliar modelos lineares, ensemble e AutoML
- **Validação robusta**: Implementar validação cruzada, análise de resíduos e diagnóstico de multicolinearidade

## Dataset

- **Fonte**: Justinas Cirtautas, pode ser acessado em: https://www.kaggle.com/datasets/justinas/nba-players-data
- **Registros**: 12.844 observações
- **Variáveis**: 17+ features incluindo métricas físicas, estatísticas de jogo e informações de draft
- **Período**: Temporadas de 1996 até 2022

## Metodologia

### 1. Análise Exploratória de Dados (EDA)
- Inspeção e limpeza dos dados
- Análise de distribuições e outliers
- Matriz de correlação e análise bivariada
- Visualizações multivariadas (pairplot)

### 2. Feature Engineering (Criação de variáveis)
- Criação de variáveis derivadas (BMI, experiência, eficiência)
- Encoding de variáveis categóricas
- Normalização de features

### 3. Modelagem de Machine Learning

#### Regressão
- Regressão Linear Simples
- Regressão Linear Múltipla
- Regressão Polinomial (grau 2 e 3)

#### Classificação
- Naive Bayes
- Regressão Logística

#### AutoML Alternativo
- Implementação de sistema automatizado
- Comparação de 6+ algoritmos de regressão
- Comparação de 7+ algoritmos de classificação
- Otimização automática de hiperparâmetros

### 4. Validação e Diagnóstico
- Validação cruzada K-Fold (k=5)
- Análise de resíduos (normalidade e homocedasticidade)
- Detecção de multicolinearidade (VIF)
- Grid Search para otimização de hiperparâmetros

## Estrutura do Repositório

```
analise_nba/
├── nba_players_analysis.ipynb              # Notebook principal (versão final)
├── nba_players_stats.csv                   # Dataset principal
├── README.md                                # Documentação do projeto
├── requirements.txt                         # Dependências Python
└── docs/                                    # Documentação adicional (se aplicável)
```

## Requisitos do Sistema

- Python 3.8+
- Jupyter Notebook ou Jupyter Lab
- 4GB+ RAM recomendado
- Processador multi-core recomendado para AutoML

## Instalação e Execução

### 1. Clone o repositório
```bash
git clone <url-do-repositorio>
cd analise_nba
```

### 2. Instale as dependências
```bash
pip install -r requirements.txt
```

### 3. Execute o notebook
```bash
jupyter notebook nba_players_analysis.ipynb
```

ou

```bash
jupyter lab nba_players_analysis.ipynb
```

## Uso

1. **Exploração inicial**: Execute as células de EDA para entender o dataset
2. **Modelagem manual**: Compare algoritmos clássicos (regressão linear, Naive Bayes)
3. **AutoML**: Execute o sistema automatizado para descobrir melhores algoritmos
4. **Validação**: Analise resultados de validação cruzada e diagnósticos
5. **Interpretação**: Consulte as análises textuais para insights de negócio

## Dependências Principais

- pandas: Manipulação de dados
- numpy: Computação numérica
- scikit-learn: Machine Learning
- matplotlib/seaborn: Visualização
- scipy: Testes estatísticos
- jupyter: Ambiente de desenvolvimento

## Licença

Este projeto é disponibilizado sob a licença MIT.