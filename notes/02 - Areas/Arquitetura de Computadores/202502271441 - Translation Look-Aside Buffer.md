---
date: 2025-02-27T14:41
tags: 
cssclasses:
  - center-titles
  - center-images
---
# Translation Look-Aside Buffer (TLB)

## Por que utilizar ele?

- Número de páginas na memória secundário é muito grande
- Tamanho excessivo da MMTT
- Se a tabela fica na memória principal => dois acessos à memória a cada cache miss

## Working set
- Nome dado para o conjunto de páginas mais prováveis de serem acessadas num dado momento devido ao princípio de localidade

## TLB
- Implementado em Hardware
- Traduz endereços virtuais para reais
- Inclui apenas páginas do working set
- Funciona como uma “cache” da MMTT

![[202502271441 - Translation Look-Aside Buffer 202502271447.excalidraw]]


## MMTT
- Implementada em Software

