# Representação do Relacionamento de Músicas Pedidas vs Tocadas (Grafo)
Grafo/Python/Metworkx

## Motivação
A fim de melhorar a interação e engajamento dos ouvintes de uma rádio e consequentemente tonar as campanhas publicitárias mais eficientes, seria possível através da teoria dos grafos identificar como se dá o relacionamento das músicas tocadas em função das músicas solicitadas de forma a identificar possíveis obras muito solicitadas que foram deixadas ao acaso assim como sugerir proativamente uma programação baseada no histórico de solicitações ? 

## Desafio

## Abordagem
1. Criar um algoritmo em python para simular uma sequência de programação de músicas aleatórias dentro de uma amostra de 100 músicas a serem tocadas na rádio (Coordenador Musical)

2. Criar um algoritmo em python para simular as solicitações dos ouvintes incrementando o 'peso' para as músicas mais solicitadas em cada sequência da programação

3. Utilizar o pacote Networkx para a estruturação dinâmica do grafo, da seguinte forma:
    - (vértice vermelha) - Representa a escolha do coordenador musical
    - (vértice azul) - Representa as solicitações dos ouvintes
    - Nas arestas está representado o número de solicitações de cada sequência

## Solução

Utilização da função DiGraph() do pacote Networkx para modelar um digrafo (grafo direcionado)

## Estrutura da Solução

## Resultado

Nesta representação é fica visível que já na segunda sequência muito embora a maioria dos pedidos estivessem apontando para a música 'Love Bluzz' a rádio reproduziu outra com menor peso e este comportamento foi replicado para várias outras músicas das sequências posteriores, desta forma a programação tende a ficar mais distante do público

<p align="center">
	<img src="Grafo1.PNG" height="50%" width="50%">
</p


Nesta outra representação é possível ver que as músicas 'Heart Of The Sunrinse' e 'America' foram recorrentemente solicitadas, entretanto não foram reproduzidas, se a rádio contasse com uma visitação estruturada poderia encerrar sua programação tocando uma ou até as duas músicas recorrentes o que agradaria aos ouvintes.

<p align="center">
	<img src="Grafo2.PNG" height="50%" width="50%">
</p


Com base nestes exemplos simples é possível perceber os vários tipos de aplicações e insights que a utilização de Grafos pode proporcionar e se bem utilizado pode trazer um bom engajamento do público alvo e consequentemente campanhas publicitárias mais abrangentes, com base neste entendimento dou como válido a hipótese inicialmente levantada.

### Algumas Considerações

- Os dados base para esta publicação são oriundos de algoritmo feito em python de escolha aleatória;
- O artigo não esgota o tema ou tem a pretensão em se aprofundar na base teórica dos Grafos
- O artigo apresenta uma solução simples e longe de outras 'features' que poderiam ser utilizadas como Centralidade, clusters, etc...




