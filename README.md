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
    - **Tamanho:**  176 KB
    - **Quantidade de Registros:**  7043
    - **Linhas x Colunas:** O conjunto de dados possui 7043 linhas x 21 colunas.
    - **Dados Faltantes:** Tratados com preenchimento de médias ou exclusão de registros.
- **Pré-processamento:**
    - Criação de uma variável binária para representar o churn.
    - Normalização das variáveis numéricas.
    - One-Hot Encoding das variáveis categóricas.
- **Análise de Métricas:**
    - Acurácia: [0.7955997161107168]
    - Precisão: [0.6693227091633466]
    - Recall: [0.450402144772118]
    - F1-Score: [0.5384615384615385]
- **Justificativa:** O Modelo 1 foi escolhido devido ao seu bom desempenho em termos de acurácia e precisão, o que é crucial para a empresa de telecomunicações na identificação de clientes propensos a cancelar seus serviços.

## Modelo 2 - Previsão de Diabetes em Pacientes
- **Objetivo do Modelo:** O Modelo 2 tem como objetivo prever se um paciente tem diabetes com base em dados clínicos, como nível de glicose, pressão sanguínea, idade, etc.
- **Conjunto de Dados:** 
    - **Origem:** [Link para o conjunto de dados](https://www.kaggle.com/uciml/pima-indians-diabetes-database)
    - **Nome:** Diabetes Prediction Dataset
    - **Tamanho:** 9 KB
    - **Quantidade de Registros:** 768
    - **Linhas x Colunas:** 768 x 9
    - **Dados Faltantes:** Tratados com imputação de médias.
- **Pré-processamento:**
    - Nenhum pré-processamento adicional.
- **Análise de Métricas:**
    - Acurácia: [0.7207792207792207]
    - Precisão: [0.6071428571428571]
    - Recall: [0.6181818181818182]
    - F1-Score: [0.6126126126126126]
- **Justificativa:** O Modelo 2 foi escolhido devido ao seu recall mais alto, o que é crucial para identificar pacientes com diabetes.

## Modelo 3 - Previsão de Fraude em Transações Financeiras
- **Objetivo do Modelo:** O Modelo 3 visa prever transações financeiras fraudulentas com base em dados de transações, incluindo informações sobre o valor da transação, horário e tipo de transação.
- **Conjunto de Dados:** 
    - **Origem:** [Link para o conjunto de dados](https://www.kaggle.com/mlg-ulb/creditcardfraud)
    - **Nome:** Credit Card Fraud Detection
    - **Tamanho:** 69 MB
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
- **Justificativa:** O Modelo 3 foi escolhido devido à sua importância na detecção de fraudes financeiras, com ênfase em recall para minimizar falsos negativos.

##Conclusão
Após avaliar detalhadamente os três modelos de classificação, cada um se destaca em sua respectiva área de aplicação. O Modelo 1 demonstrou ser a escolha ideal para a empresa de telecomunicações, oferecendo um desempenho notável em relação aos seus objetivos específicos. Por sua vez, o Modelo 2 foi identificado como altamente recomendado para aplicações médicas, atendendo eficazmente às necessidades nesse contexto.

No entanto, o Modelo 3 se destacou de maneira excepcional na área de detecção de fraudes financeiras. Sua capacidade de identificar transações fraudulentas com alta precisão é fundamental para a segurança financeira. A escolha de cada modelo foi baseada em métricas criteriosamente selecionadas para atender às demandas específicas de suas respectivas aplicações.

Em resumo, os modelos foram escolhidos de forma a otimizar o desempenho e atender às necessidades de suas respectivas áreas. Essa abordagem direcionada garante resultados precisos e confiáveis em cenários diversos, destacando a importância da seleção adequada de modelos de machine learning para aplicações específicas.





