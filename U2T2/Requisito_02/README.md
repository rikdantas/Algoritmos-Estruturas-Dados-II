# Requisito 02
No requisito 02 foi desenvolvido gráficos que ajudam a visualizar a assortatividade de cada rede escolhida. O código desenvolvido junto com os gráficos podem ser encontrados na pasta [source](https://github.com/rikdantas/Algoritmos-Estruturas-Dados-II/tree/main/U2T2/Requisito_02/source) desse repositório.

## Explicação geral dos gráficos
Os gráficos estão plotados da seguinte maneira: No eixo X está os graus dos nós e no eixo y a média dos graus dos nós vizinhos. Vale lembrar que a média é de todos os nós da rede que possuem o mesmo grau. 

A linha do meio traçada no gráfico gerado pelo código é uma linha de regressão linear que tenta mostrar a tendência ou relação entre as variáveis no gráfico de dispersão. 

Se a linha de regressão estiver subindo de forma positiva, isso indica uma correlação positiva entre as duas variáveis, o que significa que, quanto maior o grau de um nó, maior o grau médio de seus vizinhos. Se a linha estiver descendo de forma negativa, isso indicaria uma correlação negativa. Se a linha estiver plana, não haverá correlação aparente. Em outras palavras, se a regressão for positiva, quanto maior o grau do nó, maior sua assortividade e quanto menor o grau, menor a assortividade.

Essa linha é útil para visualizar a tendência geral nos dados e pode ser usada para fazer previsões simples. No entanto, a interpretação exata dos resultados depende da natureza dos dados e do contexto do problema.

## Explicação de cada gráfico

### Rede web_Google
A rede web_Google é a maior das redes escolhidas e como podemos ver no gráfico plotado, sua linha de regressão ficou negativa. Essa relação pode indicar uma estrutura hierárquica na sua rede. Nós com graus mais altos podem representar páginas "de alto nível" que têm menos vizinhos, enquanto nós com graus mais baixos podem representar páginas "de nível inferior" que são vinculadas a partir de páginas de alto nível. 

### Rede wiki_Vote
Na rede wiki_Vote, que é uma rede que contém dados de votação da wikipedia, obtivemos um gráfico com regressão positiva, mostrando que conforme o grau do nó aumenta, mais conectada a rede fica. Uma análise interessante sobre essa rede é a interação dinâmica entre os usuários mais votados, ou seja,  usuários que são reconhecidos pela comunidade (recebendo muitos votos) podem estar mais inclinados a reconhecer outros usuários que também contribuem de maneira significativa.

### Rede email_Enron
A rede email_Enron é a única rede não direcionada na lista. Os nós da rede são endereços de e-mail, e se um endereço i enviou pelo menos um e-mail para o endereço j, o grafo contém uma aresta não direcionada de i para j. O gráfico resultou em uma regressão negativa. Uma das possíveis análises para isso é: Endereços de e-mail com muitas conexões podem optar por diversificar suas comunicações, se comunicando com uma variedade de endereços de e-mail menos conectados. Isso pode resultar em uma probabilidade menor de se conectar com outros endereços altamente conectados.

### Rede web_Stanford
A web_Stanford é a rede web da universidade de Stanford, na qual Os nós representam páginas do stanford.edu e as arestas direcionadas representam hiperlinks entre elas. Assim como a rede web_Google, também obteve-se um gráfico com regressão negativa. Uma possível explicação pode ser que as páginas mais importantes deliberadamente vinculem a páginas menos importantes para fornecer informações adicionais ou contextualização para os leitores.

### Rede amazon0302
Por fim, na rede amazon 0302 que é baseada na funcionalidade 'Clientes que compraram este item também compraram' do site da Amazon, a regressão resultante foi um regressão negativa. Uma análise que pode ser feita é que produtos populares sejam comprados por uma ampla variedade de consumidores, enquanto produtos menos populares sejam comprados por consumidores que têm necessidades específicas ou interesses mais restritos.

