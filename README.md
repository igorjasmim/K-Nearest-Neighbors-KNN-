## Introdução:

Modelo supervisionado de machine learning que pode ser utilizado tanto para classificação, isto é, rotular os dados; quanto para regressão, ou seja, aproximar valores.

## Características:

- Simples
- Interpretável
- Largamente conhecido e estudado
- Razoavelmente rápido

Por conta disso é um ótimo benchmark

## Algoritmo:

- Passo 1:
    Definir um valor para K
- Passo 2:
    Definir os K vizinhos mais próximos do ponto a ser classificado de acordo com uma função de distância.
- Passo 3:
    - Se for um problema de **Regressão**:
        Calcular a **média** de todos os vizinhos.
    - Se for um problema de **Classificação**:
        Calcular a **moda** de todos os vizinhos.
- Passo 4:
    Atribuir o valor/classe ao ponto de interesse conforme cálculo do Passo 3.

## Definição do Problema:

### Dados
Os dados abaixo são referentes ao cadastro de clientes de uma empresa de investimentos com suas respectivas carteira de investimentos, que indica se esse cliente tem o perfil de investidor **Conservador**, **Moderado** ou **Agressivo**. O nosso intuito é, a partir do investimento de alguns clientes que já tem um perfil definido, estimar esse perfil para aqueles que ainda não estão classificado, afim de oferecer novos produtos que sejam mais adequados a eles.

Os dados abaixo seguem o seguinte padrão:

[**CPF**: INT, **Perfil Do Investidor**: STRING, **Carteira de Investimento**: TUPLA]

### Caso queira medir a distância utilizando a distância euclidiana

Como medir a distância euclidiana:

![image](https://github.com/user-attachments/assets/8b1f2d73-8978-4d20-9c12-904442a9c170)

### Fórmula da distância euclidiana:

![image](https://github.com/user-attachments/assets/2614dabe-ba7b-4318-9fb0-cf2c0f55818d)

