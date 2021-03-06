## Análise de regressão

A **análise de regressão** é uma técnica que permite explorar e estabelecer a relação entre uma **variável dependente** com **variáveis independentes** especificas através de um modelo matemático.
A regressão, em geral, tem como objetivo tratar de um valor que não se consegue estimar inicialmente.

### Regressão Linear

A regressão linear é chamada **linear** porque considera-se que a relação entre a variável **dependente**  e uma variável **independente** é uma função linear. Se em vez de uma, forem incorporadas várias variáveis independentes, o modelo passa a denominar-se modelo de regressão linear múltipla.

### Diagrama de dispersão

Os diagramas de dispersão ou gráficos de dispersão são representações de dados de duas ou mais variáveis que são organizadas em um gráfico. O gráfico de dispersão utiliza coordenadas cartesianas para exibir valores de um conjunto de dados.
Para as próximas explicações, será utilizado como exemplo o resultado de uma pesquisa que relaciona a taxa de mortalidade infantil de cada região do Brasil com sua respectiva taxa de analfabetismo.


| Região         | Taxa de mortalidade  infantil (_x_) | Taxa de  analfabetismo (_y_) |
|----------------|:-----------------------------------:|:----------------------------:|
| Norte          |                35,6                 |              12,7            |
| Nordeste       |                59,0                 |              29,4            |
| Sudeste        |                25,2                 |               8,6            |
| Sul            |                22,5                 |               8,3            |
| Centro - Oeste |               25,41                 |              12,4            |


Baseado nos dados da tabela acima é possível construir o gráfico abaixo onde os dados são exibidos através de pontos, cada um representando uma região, com o valor da taxa de mortalidade determinando a posição no eixo horizontal (**_x_**) e o valor da taxa de analfabetismo determinando a posição no eixo vertical (**_y_**).

#### Mortalidade infantil X Analfabetismo
![Grafico_de dispersao](https://github.com/leofernandes87/Analise-de-dados/blob/master/imagens/grafico_disp.svg)

O modelo de regressão linear nos permite estudar as relações entre essas duas variáveis numéricas contínuas, determinando se a relação é **positiva** ou **negativa** (algo que cresce ou decresce constantemente).
Observando o gráfico já é possivel determinar que neste exemplo temos uma relação **positiva**, pois quanto maior a taxa de mortalidade (eixo **x**), maior é a taxa de analfabetismo (eixo **y**).

### Método de Regressão Linear Simples

Suponhamos agora que baseados na relação das duas variáveis desejamos estimar a **taxa de analfabetismo** (**_y_**) de uma determinada região que possui uma **taxa de mortalidade** (**_x_**) de **30,0**.

A equação para nosso modelo de regressão linear simples pode ser escrita como:

<p align="center">
  <img src="https://github.com/leofernandes87/Analise-de-dados/blob/master/imagens/equation_reg_linear.svg">
</p>

onde:
- **_y_<sub>_i_</sub>** é uma variável dependente ou de resposta para o **_i_**-ésimo elemento da amostra. Esse é o valor que desejamos descobrir, no caso do exemplo acima equivale ao valor da **taxa de analfabetismo**.
- **_x_<sub>_i_</sub>** é uma variável de entrada também chamada de variável independente ou preditora, para o **_i_**-ésimo elemento da amostra. Esse será o valor dado da **taxa de mortalidade**.
- **_a_** tambem chamado de *slope*, indica quanto algo (representado pelo valor no eixo **y**) muda à medida que o valor (representado no eixo **x**) aumenta, determinando a inclinação da reta. No caso do exemplo acima, indica o quanto a taxa de analfabetismo aumenta à medida em que a taxa de mortalidade cresce. Esse é um valor desconhecido, para isso a seguinte equação deverá ser utilizada:

<p align="center">
  <img src="https://github.com/leofernandes87/Analise-de-dados/blob/master/imagens/equation_slope.svg">
</p>  
