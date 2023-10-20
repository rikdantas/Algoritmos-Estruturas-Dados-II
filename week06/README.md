# Week06
## Componentes: Paulo Ricardo Dantas e Ivamar Dantas Roque
Para as semanas 05 e 06 foram passados o estudo dos grafos e da ferramenta NetworkX para implementação dos mesmos. Nesse repositório vai ser disponbilizado o 
notebook do trabalho 1 da segunda unidade.
## Projeto 1 Unidade 2
### Objetivos

#### Objetivo Principal: Aplicar o conhecimento adquirido sobre grafos/redes na Semana 05 conforme detalhado em https://github.com/ivanovitchm/datastructure.
#### Objetivos Secundários:
  - Implementar o conhecimento da semana 5 no contexto apresentado do jogo F1 Clash.
  - Utilizar como referência os elementos citados nos slides: componentes do veículo (cards), pontuação dos pilotos, e garrafinhas (boost).

### Roteiro para implementação
  - Tarefa 01 (slides 11 e 12): Pontuação: 1,00 ponto
    1. Criar um histograma para a métrica "Team Score" com as 262.144 combinações possíveis de configuração de veículo.
    2. Estabelecer um limite no histograma que reduza significativamente as configurações possíveis.
    3.  O entregável será o código Python usado para criar o gráfico, similar ao apresentado no slide 12, junto com uma descrição do processo e a lógica para definir o filtro limitador para o "Team Score".
Toda a explicação deverá estar no arquivo README.md do repositório no Github referente ao respectivo trabalho.

  - Tarefa 02 (slide 13): Pontuação: 2,00 pontos
    1. Utilizar o filtro da Tarefa 01 e a biblioteca NetworkX para criar um gráfico similar ao apresentado no Slide 13.
    2. Escolher se o tamanho do vértice será proporcional ao "Team Score" (vértice vermelho) ou ao "Out Degree" dos cards (vértice preto).
    3. O entregável incluirá o código e a imagem do grafo. Na descrição, explicar as conclusões obtidas no contexto do jogo F1 Clash.
    4. Com o grafo do item anterior, criar um gráfico para a Função de Densidade de Probabilidade (PDF) da propriedade "Out Degree" dos vértices associados aos cards dos setups, usando além do NetworkX, a biblioteca Seaborn (KDE function).
O entregável inclui o código e a explicação contextualizada para o jogo F1 Clash sobre o que o PDF do "Out Degree" revela.

  - Tarefa 03 (slide 16): Pontuação: 1,00 ponto
    1. Criar um grafo bipartido para as garrafinhas do jogo F1 Clash e suas propriedades correspondentes, com dois grupos: Garrafinhas e Propriedades.
    2. O tamanho dos vértices das Propriedades será proporcional ao "Out Degree" dos vértices.
    3. O entregável incluirá o código para gerar o gráfico, a imagem do grafo e uma explicação contextualizando o resultado no jogo F1 Clash, utilizando a biblioteca nxviz para um layout circular similar ao Slide 16.

  - Tarefa 04 (slide 18): Pontuação: 1,00 ponto
    1. Tarefa livre.
    2. Com base no conteúdo da Semana 05, e considerando a configuração final do jogo F1 Clash derivada das peças do carro, pilotos e garrafa, propor uma solução para auxiliar um jogador a escolher uma configuração específica.
    3. O entregável será o código desenvolvido, as imagens criadas e uma explicação com as principais conclusões.


### Explicação para tarefa 1
A tarefa 1 pede um histograma que nada mais é que um gráfico que conta a ocorrência de valores com base nos dados. Nossos dados seriam todas as possíveis combinações entre oito tipos de peças, de 6 "classes" diferentes,
totalizando 262144 commmbinações diferentes. Com o histograma feito, vimos que o contexto do trabalho seria achar a melhor combinação possível, que seria a combinação que teria o maior team score, então achamos viável
manter em torno de 50 registros para continuar com o trabalho. Por tentativa e erro, foi desenvolvido um filtro que pegava apenas as combinações que possuísem o team score superior a 865 pontos.
