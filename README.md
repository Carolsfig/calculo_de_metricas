# Calculadora de Métricas de Avaliação para Modelos de Classificação

## Descrição do Projeto

Este projeto consiste em um script Python simples, totalmente compatível com o Google Colab, que calcula as principais métricas de avaliação de desempenho para modelos de aprendizado de máquina focados em tarefas de classificação.

O objetivo principal é fornecer uma ferramenta clara e didática para entender como métricas fundamentais como Acurácia, Precisão, Sensibilidade (Recall), Especificidade e F-score são derivadas dos valores de uma **Matriz de Confusão**.

## Métricas Implementadas

O script calcula as seguintes métricas:

-   **Acurácia:** A proporção de previsões corretas sobre o total de amostras.
-   **Sensibilidade (Recall):** A capacidade do modelo de identificar corretamente os casos positivos.
-   **Especificidade:** A capacidade do modelo de identificar corretamente os casos negativos.
-   **Precisão:** A exatidão das previsões positivas feitas pelo modelo.
-   **F-score (F1-Score):** A média harmônica entre a Sensibilidade e a Precisão, ideal para avaliar o balanço entre elas.

## Como Usar

A utilização do script é direta e foi pensada para ser simples.

1.  **Clone o Repositório ou Copie o Código**
    Pode-se clonar este repositório ou simplesmente copiar o código do arquivo para um ambiente Python ou uma célula do Google Colab.

2.  **Defina a Matriz de Confusão**
    No início do código, localize a seção indicada e altere os valores das quatro variáveis a seguir de acordo com o resultado do seu modelo:

    ```python
    # Passo 1: Definição da Matriz de Confusão
    # Altere os valores abaixo conforme a sua necessidade
    VP = 90  # Verdadeiros Positivos
    FN = 10  # Falsos Negativos
    FP = 5   # Falsos Positivos
    VN = 95  # Verdadeiros Negativos
    ```

3.  **Execute o Código**
    Rode o script. Os resultados serão calculados e exibidos de forma organizada no terminal ou na saída da célula.


## Fórmulas Utilizadas

As métricas são calculadas com base nas seguintes fórmulas, onde:
* **VP**: Verdadeiros Positivos
* **VN**: Verdadeiros Negativos
* **FP**: Falsos Positivos
* **FN**: Falsos Negativos
* **N**: Total de Elementos
* **P**: Precisão
* **S**: Sensibilidade

| Método        | Fórmula                           |
| :------------ | :-------------------------------- |
| Sensibilidade | $VP \ / \ (VP+FN)$                |
| Especificidade| $VN \ / \ (FP+VN)$                |
| Acurácia      | $(VP+VN) \ / \ N$                 |
| Precisão      | $VP \ / \ (VP+FP)$                |
| F-score       | $2 \times (P \times S) \ / \ (P+S)$ |

## Tecnologias Utilizadas

-   **Python 3**
-   Compatível com **Google Colab** e ambientes Jupyter.
