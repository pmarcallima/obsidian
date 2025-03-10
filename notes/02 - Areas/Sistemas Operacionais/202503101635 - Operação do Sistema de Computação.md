---
date: 2025-03-10T16:35
tags: []
---
# Operação do Sistema de Computação

- Dispositivos de I/O e a CPU podem executar de forma concorrente 
- Cada controladora de dispositivo cuida de um tipo específico de dispositivo
- Cada controladora de dispositivo tem um buffer local
- A CPU transfere dados entre os buffers locais e a RAM
- O I/O se dá entre o dispositivo e o buffer local
- A controladora informa A CPU que terminou sua operação, através de uma interrupção