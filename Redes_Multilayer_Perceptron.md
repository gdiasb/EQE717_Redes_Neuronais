# Redes *Perceptron* Multicamadas (PMC ou MLP)

## Origem: Rede Perceptron

Desenvolvida por Rosenblatt em 1958, é a estrutura mais simples para uma rede neural artificial e sua criação objetivava que a rede identificasse padrões geométricos. A rede *Perceptron* pertence à arquitetura *feedfoward*, pois o fluxo de informações parte da camada de entrada em direção à camada de saída, sem qualquer tipo de realimentação. Sua simplicidade reside no fato de possuir uma única camada constítuida por um neurônio. A Figura 1 é uma representação dessa rede com *n* variáveis (*x<sub>i</sub>*) e *n* pesos (*w<sub>i</sub>*). O único neurônio recebe o somatório das entradas ponderadas e compara com o limiar de ativação (&theta;).

<p align="center"><img src="https://image.prntscr.com/image/el5E-lPWR7uAUyRwyNTq0w.png"></p>

<div text-align="center">*Figura 1. Rede Perceptron*</div>
&nbsp;

Na figura acima foi atribuido um peso negativo fictício (*w<sub>0</sub>*) ao limiar de ativação apenas para cálculo do potencial de ativação (*u*). Esse potencial é a variável da função de ativação (*g(u)*) que retorna a única saída (*y*). Matematicamente temos a seguinte representação:

<!-- $$ u = \sum_{i=1}^{n} w_i x_i - \theta $$ --> 
<div align="center"><img src="https://render.githubusercontent.com/render/math?math=u%20%3D%20%5Csum_%7Bi%3D1%7D%5E%7Bn%7D%20w_i%20x_i%20-%20%5Ctheta%0D"></div>

<!-- $$ y = g(u) $$ --> 
<div align="center"><img src="https://render.githubusercontent.com/render/math?math=y%20%3D%20g(u)%0D"></div>

As funções de ativação, geralmente, aplicadas às redes perceptron são a função degrau (*heavside function*) ou a função degrau bipolar. Ambas são funções descontínuas e que resultam em um valor ou outro. Por exemplo, a função degrau é igual a 0, se o seu argumento *u* é menor do que 0, **ou** igual a 1, se *u* é maior do que zero. O mesmo acontece para a função degrau bipolar, porém, os valores são -1 e 1. Logo, pode-se dizer que problemas que utilizam redes perceptron são problemas que tem como resposta sim ou não, ou generalizando, *opção A* ou *opção B*. Em termos matemáticos para a função degrau, temos:

<!-- Função degrau -->
<div align="center"><img src="https://latex2png.com/pngs/fa1cd04a5ee758c812ce1badde4f7919.png"></div>

### O Treinamento do *Perceptron* 

O treinamento da rede *perceptron* tem com inspiração a Regra de Aprendizado de Hebb. No algoritmo originalmente proposto, o treinamento é dado pelas equações:

<!--w_{i}^{atual} = w_i^{anterior} + \eta(d^{(k)}- y)x_i^{(k)} --> 
<div align="center"><img src="https://render.githubusercontent.com/render/math?math=w_%7Bi%7D%5E%7Batual%7D%20%3D%20w_i%5E%7Banterior%7D%20%2B%20%5Ceta(d%5E%7B(k)%7D-%20y)x_i%5E%7B(k)%7D%0D"></div>

<!-- \theta^{atual} = \theta^{anterior} + \eta(d^{(k)}- y)(-1) -->
<div align="center"><img src="https://latex2png.com/pngs/5ee2d66d5eb17ac3d6afa1e61cb43f29.png"></div>

Em que:
* *w<sub>i</sub>* é o peso do neurônio *i*;
* *d<sup>k</sup>* é a resposta conhecida da amostra *k*;
* *y* é a resposta calculada pela rede;
* *x<sub>i</sub>* é o valor da variável de entrada *i* da amostra *k*;
* *&theta;* é o *bias*;  
* *&eta;* é a taxa de aprendizagem da rede (constante).

Se temos *n* neurônios, como na Figura 1, se pode construir os seguintes vetores:

<!-- $$ \bold{w} = [\theta w_1 w_2 ... w_n]^T $$ --> 
<div align="center"><img src="https://render.githubusercontent.com/render/math?math=%5Cbold%7Bw%7D%20%3D%20%5B%5Ctheta%20w_1%20w_2%20...%20w_n%5D%5ET%0D"></div>

<!-- $$ \bold{x}^{(k)} = [-1 x_1^{(k)} x_2^{(k)} ... x_n^{(k)}] $$ --> 
<div align="center"><img src="https://render.githubusercontent.com/render/math?math=%5Cbold%7Bx%7D%5E%7B(k)%7D%20%3D%20%5B-1%20x_1%5E%7B(k)%7D%20x_2%5E%7B(k)%7D%20...%20x_n%5E%7B(k)%7D%5D%0D"></div>

E, então, se pode reescrever as equações em termos vetoriais:

$$
\bold{w}^{atual} = \bold{w}^{anterior} + \eta(d^{(k)} - y)\bold{x}^{(k)}
$$ 


## Redes *Percepetron* Multicamadas



## Referências 

[Silva, Ivan Nunes da, Danilo Hernane Spatti, and Rogério Andrade Flauzino. “Redes neurais artificiais para engenharia e ciências aplicadas.” São Paulo: Artliber (2010).](https://artliber.com.br/amostra/redes_neurais.pdf)