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