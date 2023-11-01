# Requisito 03
No requisito 03 foi requisitado uma tabela contendo os seguintes atributos: Quantidade de vértices, Quantidade de arestas, degree_assortativity_coefficient, Quantidade de componentes conectados, Tamanho do componente gigante (GCC) e Coeficiente de clustering. O código desenvolvido para achar os atributos pode ser encontrados na pasta [source](https://github.com/rikdantas/Algoritmos-Estruturas-Dados-II/tree/main/U2T2/Requisito_03/source) desse repositório. Já a tabela vai ser disponibilizada junto com a explicação dos atributos a seguir.

## Atributos da tabela
### Quantidade de vértices
A quantidade de vértices é o mesmo que a quantidade de nós existentes no grafo. Os nós são pontos de conexão que representam entidades ou elementos. Eles são usados para construir relações entre essas entidades em um modelo de rede. Essa coluna da tabela mostra a quantidade de nós existentes em cada rede.

### Quantidade de arestas
A quantidade de arestas são as linhas que conectam os nós. As arestas podem ter atributos associados, como direção, peso ou tipo, dependendo do tipo de grafo e da aplicação. Essa coluna da tabela mostra a quantidade de arestas existentes em cada rede.

### Coeficiente de assortatividade do grau
Para entender esse coeficiente, primeiro é necessário uma explicação sobre o que é a assortatividade. A assortatividade é a métrica que mede o homofilia de uma rede. A homofilia, por sua vez, é a tendência de um nó se conectar com outro nó semelhante em alguma característica. Isso significa que nós com características comuns têm uma probabilidade maior de se conectarem entre si do que com nós que têm características diferentes.

A assortatividade do grau, analisa a tendência de nós com graus semelhantes a se conectarem entre si em uma rede. Como o grau do nó é o número de arestas que estão conectadas a esse nó, assortatividade do grau indica se nós com um alto grau tendem a se conectar com outros nós de alto grau e se nós com um baixo grau tendem a se conectar com outros nós de baixo grau.

Dado o contexto acima, o coeficiente de assortatividade é o que mede a assortatividade do grau e foi ele que foi utilizado no trabalho para a análise de assortatividade da rede. Esse coeficiente varia de -1 a 1:
- Se o coeficiente for próximo de 1, isso indica uma assortatividade positiva, o que significa que nós com graus semelhantes têm uma forte tendência de se conectar entre si.
- Se o coeficiente for próximo de -1, isso indica uma assortatividade negativa, o que significa que nós com graus diferentes têm uma tendência de se conectar.
- Se o coeficiente for próximo de 0, isso sugere uma rede onde os nós se conectam aleatoriamente, independentemente de seus graus.

### Quantidade de componentes conectados
Os componentes conectados representam subconjuntos de nós em um grafo onde cada nó está de alguma forma conectado a pelo menos um outro nó dentro desse subconjunto. Componentes conectados dividem o grafo em grupos independentes de nós que estão ligados por conexões diretas ou indiretas, e podem ser de diferentes tamanhos. Essa coluna da tabela mostra a quantidade de componentes conectados de cada rede.

### Tamanho do GCC
O Grafo do Componente Conectado Gigante (GCC) é o maior componente conectado em um grafo ou rede, ou seja, a maior porção do grafo onde todos os nós estão interligados direta ou indiretamente. Na tabela é mostrado o tamanho do maior componente conectado da rede, ou seja, quantos nós estão presentes nesse componente.

### Coeficiente de clustering
O coeficiente de clustering é uma métrica usada para avaliar a tendência dos nós em uma rede se agruparem em pequenos subgrupos interconectados, conhecidos como "clusters". Ele mede a probabilidade de que os vizinhos desse nó também sejam vizinhos uns dos outros. O coeficiente de clustering varia de 0 a 1:
- Um coeficiente de clustering igual a 0 indica que os vizinhos do nó não estão interconectados, ou seja, não formam um cluster.
- Um coeficiente de clustering igual a 1 indica que todos os vizinhos do nó estão interconectados, formando um cluster completo.


## Tabela
| | Qtd de vértices | Qtd de arestas | Coeficiente de assortatividade do grau | Qtd de componentes conectados | Tamanho do GCC | Coeficiente de clustering |
|------|------|------|------|------|------|------|
| web_Google | 875713 | 5105039 | -0.06520019402435487 | 371764 | 434818 | 0.3698306814797672 |
| wiki_Vote | 7115 | 103689 | -0.08324455771686787 | 5816 | 1300 | 0.08156344522820935 |
| email_Enron | 36692 | 183831 | -0.11076403259610496 | 1065 | 33696 | 0.49698255959950266 |
| web_Stanford | 281903 | 2312497 | -0.12201270653192699 | 29914 | 150532 | 0.3777400704132366 |
| amazon0302 | 262111 | 1234877 | 0.0026772436574012287 | 6594 | 241761 | 0.34687940756987184 |