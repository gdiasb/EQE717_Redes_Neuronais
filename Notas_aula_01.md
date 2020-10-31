# Redes Neuronais Aplicadas à Processos Químicos e Bioquímicos - Aula 01

## Introdução

Rede neuronal é um modelo matemático inspirado em sistemas biológicos neuronais teorizados. Frequentemente, a definição de redes neuronais é relacionada ao funcionamento do cérebro, i.e., há uma inspiração biológica:

>Rede neuronal é uma máquina projetada para modelar a maneira pela qual o cérebro executa uma tarefa particular ou função de interesse; a rede é usualmente implementada usando componentes eletrônicos ou é simulada por software em computador digital. (Haykin, 1999)

As redes são associadas à neurônios que possuem estruturas ramificadas de entrada (dendritos) e de saída (axônios), e este só responde se o sinal total recebido excede um certo nível de excitação. A representação matemática possui um número de variáveis de entrada, cada entrada é ponderada por um peso (o que corresponde às sinapses), soma-se os valores ponderados e caso esse seja superior a um determinado valor, então, o modelo matemático fornece uma resposta (variável de saída). Assim, a máquina aprende a partir dos dados e o aprendizado fica armazenado nos parâmetros da rede (pesos das interconexões); 


Típicas funções de ativação de um neurônio (variam entre -1 e 1):
+ Função degrau (o neurônio responde ou não);
+ Função sigmoidal;
+ Função linear;
+ Função Gaussiana (aplicada a redes RBF).

**Redes Feedfoward** 
Rede em que uma entrada segue para um neurônio e o fluxo de informações só segue para frente, i.e., não há reciclo ou retorno de informações para os neurônios.

**Redes Recorrentes** 
Diferentemente das redes feedfoward, possuem ao menos um laço de feedback (variável de entrada > neurônio > resposta > resposta retorna ao neurônio). Exemplo: Rede de Hopfield. 

## Histórico

## Fundamentos