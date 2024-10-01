# Identificação da Melhor Variável Preditiva para Reclamações de Seguro de Automóvel

## Descrição

Este projeto visa identificar a variável mais preditiva que afeta a probabilidade de um cliente realizar uma reclamação de seguro, excluindo o ID dos clientes. Para isso, foi utilizado um modelo de Regressão Logística aplicado a diversas variáveis presentes no dataset.

O dataset contém informações de clientes e suas características, como **score de crédito**, **quilometragem anual**, entre outras. O objetivo é determinar qual dessas variáveis tem a maior precisão em prever o resultado de uma reclamação de seguro.

## Pergunta Principal

**Qual é a variável mais preditiva para identificar se um cliente realizará uma reclamação de seguro?**

## Dados Utilizados

O arquivo de dados `car_insurance.csv` contém as seguintes colunas:
- `id`: Identificação do cliente.
- `outcome`: Indica se o cliente fez ou não uma reclamação.
- Várias outras variáveis relevantes, como:
  - `credit_score`: Score de crédito do cliente.
  - `annual_mileage`: Quilometragem anual do cliente.
  
## Metodologia

1. **Pré-processamento dos dados**:
   - Preenchimento de valores nulos nas colunas que possuem dados faltantes com a mediana.
   
2. **Modelagem**:
   - Utilização de regressão logística através da biblioteca `statsmodels` para testar individualmente cada variável como preditora.
   
3. **Avaliação de Precisão**:
   - Calculamos a matriz de confusão e a precisão (accuracy) de cada modelo para encontrar a variável com a maior precisão preditiva.

## Resultados

A variável com maior precisão foi armazenada no DataFrame `best_feature_df`, que contém:
- **best_feature**: Nome da melhor variável preditiva.
- **best_accuracy**: A precisão do modelo com essa variável.

## Tecnologias Utilizadas

- Python
- Pandas
- NumPy
- Statsmodels

## Como Rodar o Projeto

1. Clone este repositório: 
   ```bash
   git clone https://github.com/RafaCardinali/predictive-car-insurance-analysis.git
    ```
2. Instale as dependências:
    ```bash
    pip install pandas numpy statsmodels
    ```
3. Execute o script Python:
    ```bash
    jupyter notebook car_insurance_analysis.ipynb
    ```

## Contato

Se tiver alguma dúvida ou sugestão, sinta-se à vontade para entrar em contato:

[LinkedIn](https://www.linkedin.com/in/rafael-cardinali-213899296/)

[Email](mailto:rflcardinali@gmail.com)