# Requisito 02
No requisito 02 foi desenvolvido gráficos que ajudam a visualizar a assortatividade de cada rede escolhida. O código desenvolvido junto com os gráficos podem ser encontrados na pasta [source](https://github.com/rikdantas/Algoritmos-Estruturas-Dados-II/tree/main/U2T2/Requisito_02/source) desse repositório.

## Explicando os gráficos
Os gráficos estão plotados da seguinte maneira: No eixo X está os graus dos nós e no eixo y a média dos graus dos nós vizinhos. Vale lembrar que a média é de todos os nós da rede que possuem o mesmo grau. 

A linha do meio traçada no gráfico gerado pelo código é uma linha de regressão linear que tenta mostrar a tendência ou relação entre as variáveis no gráfico de dispersão. 

Se a linha de regressão estiver subindo de forma positiva, isso indica uma correlação positiva entre as duas variáveis, o que significa que, quanto maior o grau de um nó, maior o grau médio de seus vizinhos. Se a linha estiver descendo de forma negativa, isso indicaria uma correlação negativa. Se a linha estiver plana, não haverá correlação aparente. Em outras palavras, se a regressão for positiva, quanto maior o grau do nó, maior sua assortividade e quanto menor o grau, menor a assortividade.

Essa linha é útil para visualizar a tendência geral nos dados e pode ser usada para fazer previsões simples. No entanto, a interpretação exata dos resultados depende da natureza dos dados e do contexto do problema.