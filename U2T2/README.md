# U2T2
## Componentes: Paulo Ricardo Dantas
O trabalho 2 da segunda unidade tem como objetivos aplicar os conhecimentos das semanas 7 e 8, que são:
- Assortatividade
- Componentes conectados
- Coeficientes de clustering

O trabalho basicamente vai ser escolher 5 grafos dos datasets da universidade de stanford (<https://snap.stanford.edu/data/>) e verificar os atributos dos mesmos.

## Divisão do trabalho
- Requisito 01: Escolher 5 redes 
- Requisito 02: Fazer um gráfico birpartido sobre a assortividade para cada uma das redes e explicá-los com um texto entre 500 e 1000 palavras.
- Requisito 03: Reproduzir a tabela em markdown com base na disponibilizada pelo professor para as redes escolhidas. Disponível em: [PDF do trabalho.](https://github.com/ivanovitchm/datastructure/blob/main/lessons/week_09/U2T2.pdf)

## Requisito 01
O requisito 01 consiste em escolher 5 redes do dataset da Universidade de Stanford. Na tabela a seguir vão ser mostradas as redes escolhidas junto com seu link e descrição.

| Dataset | Descrição | 
|------|------|
| [Google web graph](https://snap.stanford.edu/data/web-Google.html) | Os nós representam páginas da web, e as arestas direcionadas representam hiperlinks entre elas. Os dados foram divulgados em 2002. |
| [Wikipedia vote network](https://snap.stanford.edu/data/wiki-Vote.html) | A rede contém todos os dados de votação da Wikipedia desde o início da Wikipedia até janeiro de 2008. Os nós na rede representam os usuários da Wikipedia, e uma aresta direcionada de um nó i para um nó j representa que o usuário i votou no usuário j. |
| [Enron email network](https://snap.stanford.edu/data/email-Enron.html) | Esses dados foram originalmente tornados públicos e postados na web pela Comissão Reguladora de Energia Federal durante sua investigação. Os nós da rede são endereços de e-mail, e se um endereço i enviou pelo menos um e-mail para o endereço j, o grafo contém uma aresta não direcionada de i para j. |
| [Stanford web graph](https://snap.stanford.edu/data/web-Stanford.html) | Os nós representam páginas da Universidade de Stanford (stanford.edu) e as arestas direcionadas representam hiperlinks entre elas. Os dados foram coletados em 2002. |
| [Amazon product co-purchasing network](https://snap.stanford.edu/data/amazon0302.html) | A rede foi coletada rastreando o site da Amazon. Ela é baseada na funcionalidade 'Clientes que compraram este item também compraram' do site da Amazon. Se um produto i é frequentemente comprado junto com o produto j, o grafo contém uma aresta direcionada de i para j. Os dados foram coletados em 2 de março de 2003. |

O código que vai ser usado como base para baixar os datasets e criar os grafos pode ser encontrado [aqui](https://github.com/rikdantas/Algoritmos-Estruturas-Dados-II/blob/main/U2T2/source/U2T2_Requisito_01.ipynb).

## Requisito 02
O requisito 02 consiste em fazer um gráfico sobre assortatividade. Para vê-lo basta clicar [aqui](https://github.com/rikdantas/Algoritmos-Estruturas-Dados-II/tree/main/U2T2/Requisito_02).