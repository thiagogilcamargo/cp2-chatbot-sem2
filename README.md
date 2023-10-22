# Checkpoint 2 - Modelos de Classificação

**Aluno:** [Thiago Gil Camargo]

**RM:** [551211]

## Introdução
Este repositório contém o relatório do Checkpoint 2 do curso de ADS. O objetivo do checkpoint é a implementação de três modelos de classificação, análise de dados e métricas associadas. Foram utilizados conjuntos de dados apropriados para cada modelo, e o desempenho dos modelos foi avaliado.

## Modelo 1 - Previsão de Churn em uma Empresa de Telecomunicações
- **Objetivo do Modelo:** O Modelo 1 visa prever se um cliente de uma empresa de telecomunicações irá cancelar seu serviço (churn) com base em informações demográficas e comportamentais do cliente.
- **Conjunto de Dados:** 
    - **Origem:** [Link para o conjunto de dados](https://www.kaggle.com/blastchar/telco-customer-churn)
    - **Nome:** Telecom Churn Dataset
    - **Tamanho:** 1 MB
    - **Quantidade de Registros:**  7043
    - **Linhas x Colunas:** O conjunto de dados possui 7043 linhas x 21 colunas.
    - **Dados Faltantes:** Tratados com preenchimento de médias ou exclusão de registros.
- **Pré-processamento:**
    - Criação de uma variável binária para representar o churn.
    - Normalização das variáveis numéricas.
    - One-Hot Encoding das variáveis categóricas.
- **Análise de Métricas:**
    - Acurácia: [0.8218594748048261]
    - Precisão: [0.6871165644171779]
    - Recall: [0.6005361930294906]
    - F1-Score: [0.6409155937052933]
    **Modelo**: Regressão Logística
- **Justificativa:** A regressão logística é um modelo simples e interpretable que pode ser eficaz na previsão de churn em empresas de telecomunicações. É uma escolha sólida quando a precisão e a interpretabilidade são essenciais.

# Modelo 2 - Previsão de Sobrevivência no Titanic
- **Objetivo do Modelo:** O Modelo 2 tem como objetivo prever a sobrevivência dos passageiros a bordo do RMS Titanic com base em dados como classe da passagem, sexo, idade, entre outros.
- **Conjunto de Dados:** 
    - **Origem:** [Link para o conjunto de dados](https://www.kaggle.com/c/titanic)
    - **Nome:** Titanic: Machine Learning from Disaster
    - **Tamanho:** 163 KB (train.csv), 82.3 KB (test.csv)
    - **Quantidade de Registros (Treinamento):** 891
    - **Quantidade de Registros (Teste):** 418
    - **Colunas:** 12
    - **Dados Faltantes (Treinamento):** Tratados com imputação de médias e modas.
    - **Dados Faltantes (Teste):** Tratados com imputação de médias e modas.
- **Pré-processamento:**
    - Preenchimento de valores faltantes em colunas relevantes (idade, tarifa, etc.).
    - Mapeamento da coluna "Sex" para valores numéricos.
- **Análise de Métricas:**
    - Acurácia: [0.8100558659217877]
    - Precisão: [0.7727272727272727]
    - Recall: [0.6857142857142857]
    - F1-Score: [0.726027397260274]
- **Modelo:** Gradient Boosting Classifier
- **Justificativa:** O modelo Gradient Boosting Classifier foi escolhido por sua eficácia em problemas de classificação e sua capacidade de lidar com recursos numéricos e categóricos.


## Modelo 3 - Previsão de Fraude em Transações Financeiras
- **Objetivo do Modelo:** O Modelo 3 visa prever transações financeiras fraudulentas com base em dados de transações, incluindo informações sobre o valor da transação, horário e tipo de transação.
- **Conjunto de Dados:** 
    - **Origem:** [Link para o conjunto de dados](https://www.kaggle.com/mlg-ulb/creditcardfraud)
    - **Nome:** Credit Card Fraud Detection
    - **Tamanho:** 150 MB
    - **Quantidade de Registros:** 284.807
    - **Linhas x Colunas:** 284807 x 31
    - **Dados Faltantes:** Não há dados faltantes.
- **Pré-processamento:**
    - Padronização das variáveis numéricas.
- **Análise de Métricas:**
    - Acurácia: [0.9995611109160493]
    - Precisão: [0.974025974025974]
    - Recall: [0.7653061224489796]
    - F1-Score: [0.8571428571428571]
    - **modelo:** RandomForest
- **Justificativa:** A detecção de fraudes financeiras é uma tarefa crítica que requer modelos robustos e capazes de lidar com conjuntos de dados desbalanceados. O Random Forest se destaca nesse contexto devido ao seu desempenho sólido e versatilidade. Sua capacidade de lidar com dados desbalanceados, identificar padrões complexos e fornecer uma alta precisão na detecção de fraudes o torna uma escolha ideal. Além disso, a seleção criteriosa de variáveis e o pré-processamento adequado dos dados contribuíram para a eficácia do modelo na identificação de transações fraudulentas, priorizando a segurança financeira.


- **Escolha do melhor modelo:**Com base nas métricas de desempenho, o "Modelo 3 - Previsão de Fraude em Transações Financeiras (Random Forest)" se destaca por sua excepcional precisão e recall na detecção de fraudes. No entanto, a escolha do melhor modelo deve ser direcionada pelo problema específico que você deseja resolver. Se a detecção de fraudes financeiras é a sua principal prioridade, o Modelo 3 é a escolha ideal. Se você está lidando com outros cenários, como previsão de sobrevivência ou churn, o Modelo 1 ou 2 pode ser mais apropriado, dependendo dos objetivos do projeto.

Portanto, não há um "melhor" modelo em geral, mas sim um modelo mais adequado para um contexto específico.
#Conclusão
Após uma análise detalhada dos três modelos de classificação e suas respectivas áreas de aplicação, fica evidente que a escolha criteriosa de um modelo de machine learning desempenha um papel crucial no sucesso de uma solução. Cada modelo se destacou em sua área de expertise, demonstrando ser a escolha ideal para aplicações específicas.

O Modelo 1, baseado em Regressão Logística, provou ser altamente eficaz na previsão de churn em uma empresa de telecomunicações. Sua capacidade de identificar clientes propensos a cancelar seus serviços é fundamental para a retenção de clientes e o planejamento de estratégias de negócios.

Para aplicações médicas, o Modelo 2 apresentou resultados promissores. Sua capacidade de prever a presença de diabetes com base em dados clínicos, como níveis de glicose e pressão sanguínea, oferece suporte valioso a profissionais de saúde na identificação precoce da condição.

No entanto, o destaque vai para o Modelo 3, dedicado à detecção de fraudes em transações financeiras. Sua excepcional precisão na identificação de transações fraudulentas é vital para a segurança financeira. A seleção criteriosa de variáveis, o pré-processamento adequado e a escolha de métricas focadas na minimização de falsos negativos contribuíram para seu desempenho notável.

Em suma, a escolha de um modelo de machine learning deve ser guiada pela compreensão das necessidades específicas de cada aplicação. Esta abordagem direcionada garante que os resultados atendam com precisão os objetivos de cada domínio. Os modelos aqui apresentados ilustram como a seleção criteriosa de modelos é essencial para alcançar resultados precisos e confiáveis em cenários diversos.



