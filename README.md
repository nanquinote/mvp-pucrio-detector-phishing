# Classificador de Phishing
Código do projeto para a Sprint de Machine Learning do curso de pós-graduação em Ciência de Dados e Analytics da PUC-Rio.

# Classificação de URLs Fraudulentas com Machine Learning

## Sobre o Projeto
Este projeto desenvolve um modelo de **Machine Learning** para identificar URLs fraudulentas (phishing) e diferenciá-las de URLs legítimas. O objetivo é aumentar a segurança digital ao prevenir fraudes e proteger dados sensíveis.

🔗 **Acesse o Notebook no Google Colab:** [Clique aqui](https://colab.research.google.com/drive/1zIF2C62nHFAeUX311wuxmScag00rnxeT?authuser=0)

---

## Contexto
O phishing é uma prática criminosa em que sites falsos são usados para enganar usuários e roubar informações pessoais ou financeiras. Com o aumento das ameaças digitais, um modelo eficiente para identificar URLs suspeitas é essencial.

### Problema
Classificar URLs em **legítimas** ou **fraudulentas** com base em características extraídas delas, como comprimento, presença de HTTPS e padrões no domínio.

---

## Objetivo
Criar e avaliar um modelo de Machine Learning para identificar URLs fraudulentas com alta precisão e capacidade de generalização.

---

## Dataset
O dataset utilizado é o **"PhiUSIIL Phishing URL (Website)"**, que contém diversas características de URLs, incluindo indicadores de segurança e padrões estruturais.

### Dicionário de Dados
Os dados incluem colunas como:
- `URL`: A URL completa sendo analisada.
- `DomainLength`: Comprimento do domínio principal.
- `IsHTTPS`: Indica se a URL usa HTTPS.
- `NoOfSubDomain`: Número de subdomínios presentes.
- `label`: Rótulo da URL (1 - legítima, 0 - phishing).
- [Veja o dicionário completo no notebook](https://colab.research.google.com/drive/1zIF2C62nHFAeUX311wuxmScag00rnxeT?authuser=0).

---

## Tecnologias e Bibliotecas Utilizadas
- **Python**: Linguagem principal.
- **Bibliotecas**:
  - Manipulação de Dados: `pandas`, `numpy`
  - Visualização: `matplotlib`, `seaborn`, `plotly`
  - Machine Learning: `sklearn`, `xgboost`
  - Balanceamento de Dados: `imblearn`

---

## Etapas do Projeto
1. **Pré-processamento dos Dados**:
   - Limpeza e tratamento de dados.
   - Balanceamento utilizando o algoritmo **SMOTE**.
2. **Análise Exploratória**:
   - Visualizações para entender a distribuição e padrões dos dados.
3. **Seleção de Features**:
   - Uso de técnicas como `SelectKBest` e análise de relevância das features.
4. **Modelagem**:
   - Treinamento de modelos como:
     - Regressão Logística
     - Random Forest
     - SVM
     - XGBoost
5. **Avaliação do Modelo**:
   - Métricas como `accuracy`, `f1-score` e `AUC`.
   - Validação cruzada e curva de aprendizado.

---

1. Clone o repositório:
   ```bash
   git clone <URL_DO_REPOSITORIO>

