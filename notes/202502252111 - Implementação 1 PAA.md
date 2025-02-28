---
date: 2025-02-25T21:11
tags: []
---
A ideia é a seguinte:
Para gerar um grafo aleatória conexo:

	- Gerar uma árvore a partir da quantidade de vértices dada pelo usuário
	- Adicionar arestas aleatórias de forma que restem apenas 2 vértice grau ímpar ou todos de grau par

Como saber se os graus bateram a quantidade certa?

- Ter na classe vértice um count de arestas
- Será necessário sempre verificar todos os vértices?
	  - Existe alguma organização que facilita essa adição aleatória?
	  - Talvez uma lista de vértices de grau impar?
	  - Talvez