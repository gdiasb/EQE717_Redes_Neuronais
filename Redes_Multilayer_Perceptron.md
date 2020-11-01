# Redes *Perceptron* Multicamadas (PMC ou MLP)

' Referência: [Silva, Ivan Nunes da, Danilo Hernane Spatti, and Rogério Andrade Flauzino. “Redes neurais artificiais para engenharia e ciências aplicadas.” São Paulo: Artliber (2010).](https://artliber.com.br/amostra/redes_neurais.pdf)'

## Origem: Rede Perceptron

Desenvolvida por Rosenblatt em 1958, é a estrutura mais simples para uma rede neural artificial e sua criação objetivava que a rede identificasse padrões geométricos. A rede *Perceptron* pertence à arquitetura *feedfoward*, pois o fluxo de informações parte da camada de entrada em direção à camada de saída, sem qualquer tipo de realimentação. Sua simplicidade reside no fato de possuir uma única camada constítuida por um neurônio. A Figura 1 é uma representação dessa rede com *n* variáveis (*x<sub>i</sub>*) e *n* pesos (*w<sub>i</sub>*). O único neurônio recebe o somatório das entradas ponderadas e compara com o limiar de ativação (&theta;).

![Figura 1. Rede *Perceptron*](https://image.prntscr.com/image/el5E-lPWR7uAUyRwyNTq0w.png)

*Figura 1. Rede Perceptron*
&nbsp;

Na figura acima foi atribuido um peso negativo fictício (*w<sub>0</sub>*) ao limiar de ativação apenas para cálculo do potencial de ativação (*u*). Esse potencial é a variável da função de ativação (*g(u)*) que retorna a saída (*y*). Matematicamente temos a seguinte representação:

$$u = \sum_{i=1}^{n} w_i x_i - \theta$$


$$y = g(u) $$
