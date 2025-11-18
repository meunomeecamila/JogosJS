# ⛵ Navio no Mar Infinito (Infinite Sailing)

### Um projeto de simulação visual simples que utiliza o conceito de scrolling background para criar a ilusão de um navio navegando em um mar infinito, desenvolvido com p5.js.

Este projeto foca em dois elementos visuais principais: o **Navio (ship)** e o **Mar (sea)**. A principal mecânica implementada é o **scrolling background (fundo que se repete)**, que faz com que o sprite do mar se mova horizontalmente e se reinicie infinitamente, dando a impressão de que o navio está sempre navegando para frente.

O navio possui uma **animação** simples (alternando entre `ship1.png` e `ship2.png`), o que adiciona vida ao cenário e reforça o efeito de movimento contínuo. 

---

## ✨ Características do Jogo

* **Scrolling Background (Mar Infinito):** O sprite do mar (`mar`) tem uma velocidade horizontal constante (`mar.velocityX = -5`). Quando a posição X do mar (`mar.x`) é menor que zero (o sprite sai da tela), ele é reiniciado para a posição inicial (`mar.width/8`), criando um loop visual ininterrupto.
* **Animação do Navio:** O navio (`navio`) utiliza o recurso `loadAnimation` para alternar entre as imagens (`ship1.png`, `ship2.png`), simulando o balanço ou o movimento da navegação.
* **Uso de Sprites:** O jogo é construído inteiramente com a biblioteca de sprites do p5.js (`createSprite`, `addImage`, `addAnimation`).

---

## 🕹️ Como Jogar (Interação)

Esta é uma simulação de visualização passiva:

1.  **Início:** Ao executar o código, o mar começará a se mover imediatamente.
2.  **Observação:** Observe o navio animado e como o fundo do mar se repete continuamente para manter a ilusão de viagem infinita.

---

## ⚙️ Tecnologias Utilizadas

* **JavaScript:** Linguagem principal de programação.
* **p5.js (Bibliotecas de Sprites):** Framework principal para:
    * Criação do canvas e do loop de desenho (`draw`).
    * Gerenciamento de sprites (`createSprite`, `drawSprites`).
    * Carregamento de imagens e animações (`loadImage`, `loadAnimation`).