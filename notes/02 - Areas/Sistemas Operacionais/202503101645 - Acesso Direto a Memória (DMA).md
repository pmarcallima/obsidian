---
date: 2025-03-10T16:45
tags: 
cssclasses:
  - center-images
  - center-titles
---
# Acesso Direto a Memória (DMA)

- Usado para permitir a dispositivos de I/O de alta velocidade transmitirem informação em velocidade comparável à da memória.
- Controladora do dispositivo transfere blocos de dados do buffer diretamente à memória principal, sem a intervenção da CPU
- Apenas uma interrupção é gerada por bloco, ao invés de uma interrupção por byte ( ao invés de escrever byte a byte, é escrito bloco a bloco)