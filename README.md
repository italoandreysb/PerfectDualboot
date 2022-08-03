# PerfectDualboot
The right way to do it.

Clica com o botão direito na partição:

Criar partição:

Tamanho: 16000MB

Tipo: Primária (todas)

Local: inicio deste espaço (todas)

Usar como: Area de troca SWAP

---

Tamanho: 512MB
Usar como: Partição de sistema EFI

Tamanho:total (o que restou)

Usar como: Sistema de arquivos com "Journaling" ext4

Ponto de montagem: /

---

Dispositivo no qual instalar o carregador de inicialização:

Selecionar a EFI de 512MB que criamos (pelo nome do dispositivo)

Clica em instalar e pronto

Referência: [Youtube](https://www.youtube.com/watch?v=yGk3E6l8vb0)
