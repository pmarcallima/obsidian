---
date: 2025-03-10T17:27
tags: 
cssclasses:
  - center-images
  - center-titles
---
# Arquitetura Geral do Sistema

- Visto que as instruções de I/O são privilegiadas, como o usuário executa I/O?
- Chamadas ao Sistema (System calls) 
	- método usado por um processo para requisitar uma determinada ação ao S.O.
		- Usualmente é na forma de exceção para uma posição específica do vetor de interrupções
		- O controle passa a uma rotina de serviço no S.O. e o bit de modo é trocado para modo monitor
		- O monitor verifica se os parâmetros são corretos e válidos, executa a requisição e retorna o controle para a instrução seguinte à chamada ao sistema