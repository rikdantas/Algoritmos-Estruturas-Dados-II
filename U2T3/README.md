# U2T3
## Componentes: Ivamar Dantas Roque e Paulo Ricardo Dantas
O trabalho 3 da segunda unidade tem como objetivos aplicar os conhecimentos das semanas 10, 11 e 12, que são:
- Excentricidade, Diametro, Periferia, Raio e Centralidade
- *Degree, Closeness, Betweenness and Eigenvector Centrality*
- *Centrality Distributions*
- *Core Decomposition*
- Biblioteca wikipedia para criação de redes dirigidas
- Introdução a ferramenta Gephi

O trabalho basicamente vai ser escolher 4 sementes (páginas da wikipedia) fazer um rede dirigida para cada uma das sementes e depois mesclar essas redes. 

## Divisão do trabalho
- Requisito 01: 
    - Gerar uma rede (grafo) dirigida a partir dos links das páginas do Wikipédia
considerando a fusão de 4 SEEDs (páginas iniciais)
    - As SEEDs deverão ser diferentes daquela fornecida no exemplo da semana 11.
Limitar o nível de profundidade da rede para 2 (similar ao que foi demonstrado
em sala de aula). 

- Requisito 02: A partir da rede construída gerar uma figura similar utilizando o Gephi. Adote um layout que seja razoável perceber a diferença entre as cores do vértices. As figuras devem ser acompanhadas de descrições/explicações.

- Requisito 03: A partir da rede construída gerar uma figura similar considerando o in-Degree dos
vértices da rede. A figura deverá ser acompanhada de explicações/descrições.

- Requisito 04: A partir da rede construída gerar uma figura similar no gephi destacando o k-core e o k-shell da rede. O layout é de livre escolha. Os vértices devem ter um tamanho
proporcional a propriedade in-degree. A figura deverá estar acompanhada de descrição/explicação.

- Requisito 05: A rede deverá estar em produção de forma análoga ao explicado na Semana 12. As cores deverão ser relacionadas ao critério de comunidade e o tamanho do vértice a métrica in-degree. 


# Resolução do trabalho
## Requisito 1
A primeira parte da resolução é escolher as 4 páginas da wikipedia que vão ser usadas para gerar as redes. As páginas foram escolhidas com um critério base, para que elas tenham uma ligação, mas não diretamente.

As redes escolhidas foram: Golden State Warriors, Olympic Games, Nike Inc e Tissot. Na tabela a seguir vão ser disponibilizados os links como referência.

| Página | Link | 
|------|------|
| Golden State Warriors | https://en.wikipedia.org/wiki/Golden_State_Warriors |
| Olympic Games  | https://en.wikipedia.org/wiki/Olympic_Games |
| Nike, Inc. | https://en.wikipedia.org/wiki/Nike,_Inc. |
| Tissot | https://en.wikipedia.org/wiki/Tissot |

Para transformar essas páginas em redes, foi utilizado a biblioteca da wikipedia. O código utilizado foi o [U2T3_Requisito_1.ipynb](https://github.com/rikdantas/Algoritmos-Estruturas-Dados-II/blob/main/U2T3/source/U2T3_Requisito_1.ipynb). Porém a execução desse código é demorado, tendo células que demoraram cerca de 50 minutos para executar, então foram baixados os arquivos graphml resultantes desse notebook, e foram upados em um drive, para que se alguém for reproduzir esse repositório, não precise rodar novamente o notebook por horas. 

O notebook [U2T3_Compose.ipynb](https://github.com/rikdantas/Algoritmos-Estruturas-Dados-II/blob/main/U2T3/source/U2T3_Compose.ipynb) importa as 4 redes e usa o método compose da biblioteca networkx para uní-las em apenas uma (*fgraph.graphml*). Note que a quantidade de nós da rede final não é exatamente a soma da quantidade de nós de cada uma das redes, isso devido ao fato que entre essas redes existem alguns nós e arestas que são comuns, que é uma das finalidades desse trabalho, achar nós e arestas comuns em diferentes redes. As redes resultantes podem ser encontradas nesse [link](https://drive.google.com/drive/folders/1Q_kZAwqZ8u2u9eWlB67fhz2Qq-nbzjLf?usp=drive_link).