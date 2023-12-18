# U3T1
## Componentes: Emanoel Batista Pereira Filho, Ivamar Dantas Roque, Paulo Ricardo Dantas

Foram disponibilizados vários projetos para a terceira unidade. A tarefa que a gente escolheu foi a de usar o Osmnx para escolher pontos turísticos de uma cidade e usar um algoritmo para achar o menor caminho entre esses pontos. A seguir vão ser descritos alguns resquisitos necessários para o trabalho:

- Seleção da Cidade e Pontos Turísticos
- Implementação do Algoritmo de Simulated Annealing
- Desenvolvimento de uma Interface de Usuário baseada no Folium e Osmnx
- Simulação e Teste de Roteiros
- Visualização do Roteiro


# Resolução do trabalho

Antes de começar a resolução é necessário que se faça a devida referência, pois os códigos que vão ser usados para o nosso estudo de caso estão disponíveis no github do finlandês Ossi Myllymäki, mais especificamente nesse [repositório](https://github.com/omyllymaki/conquering-seven-hills/tree/main).

# Funcionamento do OSMNX

O OSMnx (OpenStreetMap and NetworkX) é uma biblioteca Python que facilita a recuperação, a modelagem e a visualização de dados de redes urbanas a partir do OpenStreetMap (OSM). Ele é construído sobre a biblioteca NetworkX, que é usada para manipular estruturas de dados de grafo em Python.

Aqui estão os passos básicos de como o OSMnx funciona:

Download de dados OSM:

O OSMnx permite que você baixe dados de ruas, redes de transporte público e outros elementos urbanos diretamente do OpenStreetMap.
Você pode fornecer coordenadas geográficas ou um nome de lugar (como uma cidade) para extrair os dados.

Criação de Grafos:
O OSMnx converte os dados OSM em um grafo direcionado ponderado, onde os nós representam interseções ou pontos de interesse, e as arestas representam ruas ou caminhos entre esses nós.
As características das ruas, como comprimento, tipo de rua e direção, são atribuídas às arestas.

Análise do Grafo:
Uma vez criado o grafo, você pode realizar várias análises, como encontrar o caminho mais curto entre dois pontos, calcular a centralidade dos nós, identificar ciclos, entre outros.
O OSMnx fornece uma variedade de funções para analisar e visualizar características do grafo.

Visualização:
O OSMnx oferece ferramentas para visualizar graficamente a rede urbana que você extraiu do OSM.
Você pode gerar mapas que mostram a topologia da rede, a distribuição de tipos de ruas, a conectividade entre diferentes partes da cidade, entre outras informações.

