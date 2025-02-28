---
date: 2025-02-25T10:51
tags: 
cssclasses:
  - center-titles
---
# Algoritmo de Tarjan para Pontes

Dado um grafo G = (V , E) não direcionado , ele é chamado de bridge-connected caso for conectado por arestas que não são pontes.
Os componentes conexos (bridge-connected) são o maior número de subgrafos conexos.
Uma spanning tree de um grafo é um subgrafo que é uma árvore e contém todos os vértices de um grafo.
Uma arvore com raiz direcionada é um grafo direcionando com uma única raiz de modo que exista um único caminho da raiz para qualquer outro vértice da árvore
A existência de uma aresta (v,w) em uma árvore com raiz direcionada é dada por v -> w e a existência de um caminho de v para v \*-> w, se v->w, v é o pai de w e w é um filho de v
se v \*-> w, v é um ancestral de w e w é um descendente de v


# Para achar as pontes

Para achar todas as pontes de um grafo não direcionado G
T = spanning tree (G)
Converter T para uma árvore com raiz direcionado escolhendo um vértice arbitrário r de T e para todo caminho de r para um vértice v in T, direcionando as arestas desse caminho para que seja um caminho direcionado de r para v
uma aresta não-arvore (v,w) é chamada de v -- w
O número de vértices T de 1 pra V em pós-ordem, essa ordem corresponde ao seguinte código:


