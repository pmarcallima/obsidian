---
date: 2025-03-10T16:52
tags: 
cssclasses:
  - center-titles
  - center-images
---
# Operação em Modo Dual

- O compartilhamento de recursos requer que o S.O. garanta que um programa não prejudique a execução dos demais
- Um bit acrescentado ao hardware permite diferenciar dois modos de operação:
	- Modo Usuário (execução a favor do usuário)
	- Modo Monitor(Modo supervisor ou Modo sistema) (execução em favor do S.O.)

# Operação

- Bit de Modo indica o modo corrente: monitor(0) ou usuário(1)
- Quando uma interrupção ou exceção acontece, o hardware muda para o modo monitor

![[202503101652 - Operação em Modo Dual 202503101656.excalidraw]]

**Instruções privilegiadas só podem ser executadas em modo monitor**