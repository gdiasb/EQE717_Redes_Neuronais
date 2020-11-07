2. Defina:

**a)** Redes Neuronais;
  
  >Rede neuronal é uma máquina projetada para modelar a maneira pela qual o cérebro executa uma tarefa particular ou função de interesse; a rede é usualmente implementada usando componentes eletrônicos ou é simulada por software em computador digital. (Haykin, 1999)

**b)** Métodos de Treinamento Supervisionados e Não Supervisionados;
A diferença entre os dois métodos está no conjunto de dados para treinamento da rede neuronal. Métodos supervisionados utilizam conjunto de dados compostos por variáveis de entradas (*x<sub>i</sub>*) e resultados conhecidos (*y*). No método não supervisionado, o conjunto de dados de treinamento contém **apenas** os valores das variáveis de entrada e o método tenta aprender ser um professor (dados de saída). 

Métodos de treinamento supervisionado são aplicados a problemas de:
* Classificação;
* Regressão;

Métodos de treinamento não-supervisionados são aplicados a problemas de:
* Clusterização;
* Redução de dimensionalidade;
* Detecção de *outliers*

**c)** *Backpropagation*;
É um algoritmo em que dado o cálculo do erro ocorrido na camada de saída da rede neural, recalcula o valor dos pesos da camadas anteriores a partir da última até chegar à camada de entrada (i.e., de trás para frente). Suas etapas são:

1. Atribuir, inicialmente, valores aleatórios aos pesos da rede;
2. Fornecer os dados de entrada à rede, calcular a resposta de saída e comparar os valores dos resultados predito e esperado. Matematicamente:

<!-- $$ E(y_{obj}, y_{pred}) = \sum_{i = 1}^N (y_{obj} - y_{pred})^2 $$ --> 

<div align="center"><img src="https://render.githubusercontent.com/render/math?math=E(y_%7Bobj%7D%2C%20y_%7Bpred%7D)%20%3D%20%5Csum_%7Bi%20%3D%201%7D%5EN%20(y_%7Bobj%7D%20-%20y_%7Bpred%7D)%5E2%0D"></div>