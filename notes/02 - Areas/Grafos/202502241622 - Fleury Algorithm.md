---
date: 2025-02-24T16:22
tags: 
cssclasses:
  - center-titles
---
# Algoritmo de Fleury

## Para que serve?

- Encontrar Caminhos Eulerianos em Grafos
## Pré-requisitos e condições:

- O grafo deve possuir todos seus vértices com graus pares, não necessariamente iguais ou 2 de grau ímpar
- Caso possua todos graus pares, deve-se começar e terminar pelo mesmo vértice
## Pseudocódigo:
### 2 graus impares

1. Escolher um dos vértices de grau impar
2. Andar para algum vértice vizinho partindo de uma aresta não ponte
3. repetir o passo 2 até não possuir mais de 1 aresta possível
### Todos graus pares:
1. Escolher qualquer vértice do grafo
2. Andar para algum vértice vizinho partindo de uma aresta não ponte
3. repetir o passo 2 até não possuir mais de 1 aresta possível

## Como encontrar pontes?

[[202502241806 - Tarjan Algorithm]]
- [[Naive]]