---
date: 2025-03-10T15:44
tags: 
cssclasses:
  - center-titles
  - center-images
---
# Sistemas em Batch(Lote)

- Operador comanda a submissão de tarefas(jobs)

- Usuário != operador

- Tarefa na forma de cartões perfurador

- Tempo de configuração era reduzido, reunindo-se tarefas similares

- Sequenciamento automático, controle transferido automaticamente de um job para outro

- S.O. rudimentar

- Monitor residente
	 - controle inicial
	 - controle transferido para o job
	 - quando ob termina, o controle é devolvido ao monitor

![[202503101544 - Sistemas em Batch 202503101546.excalidraw]]


## Problemas:

- Baixa-Perfomance
- CPU e I/O não podiam ser sobrepostas
- CPU ficava ociosa
- A leitura dos cartões era muito lenta

## Solução:

- Operação off-line
- Jobs carregados de unidades de fita para a memória
- A leitura de cartões e tarefas de impressão eram feitas off-line
## Job Pool

- Estrutura de dados que permite selecionar qual job será executado a seguir, para aumentar o uso da CPU.