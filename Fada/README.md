# ✨ Estrela Cadente da Fada (Fairy Star Drop)

### Um jogo temático de contos de fadas que simula a queda de uma estrela sob a gravidade, desenvolvido com Matter.js e p5.js, com foco em sprites e áudio.

Este projeto estabelece um cenário noturno (`starNight.png`) onde uma **Estrela (Star)** é suspensa no céu. O objetivo principal do jogo é provavelmente **liberar a estrela** em um momento específico, permitindo que ela caia (como uma estrela cadente) em um local de destino.

A estrela é inicialmente mantida estática, mas pode ser liberada para cair livremente, utilizando o motor de física do **Matter.js** para simular o movimento de queda e colisão. O código também sugere a inclusão de uma **Fada** (com animação e som) que interage com a estrela, adicionando um elemento de história ao jogo. 

---

## ✨ Características do Jogo

* **Física de Queda:** A estrela é um corpo circular (`starBody`) com restituição (`restitution: 0.5`) que espera ser liberado do estado estático (`isStatic:true`) para cair sob a influência da gravidade do Matter.js.
* **Ambientação:** Utiliza sprites e imagens de fundo (`starNight.png` e `star.png`) para criar uma atmosfera noturna mágica.
* **Componentes de Conto de Fadas:** O código prevê a inclusão de um sprite para a **Fada** (`fadaSprite`) e um som de áudio (`vozFada`), que são centrais para a narrativa do jogo.
* **Canvas Grande:** O jogo utiliza uma tela de 800x750 pixels, ideal para um cenário noturno amplo.

---

## 🕹️ Como Jogar (Interação Esperada)

Embora o código de interação (liberar a estrela e mover a fada) não esteja completo, as etapas prováveis seriam:

1.  **Observação:** O jogo começa com a estrela suspensa e a fada se movendo ou pairando.
2.  **Interação:** O jogador deve pressionar uma **tecla específica** (não definida no código) para mudar a propriedade `isStatic` da estrela para `false`.
3.  **Objetivo:** O jogador pode precisar guiar a fada ou cronometrar a queda da estrela para que ela caia em um ponto específico da tela.

---

## ⚙️ Tecnologias Utilizadas

* **JavaScript:** Linguagem principal.
* **Matter.js:** Biblioteca de física 2D para gerenciar a estrela como um corpo rígido e simular a queda livre.
    * Módulos chave: `Engine`, `World`, `Bodies`, `Body`.
* **p5.js (Implícito):** Framework de desenho e renderização (criação de canvas, carregamento de imagens e loop de jogo).
* **Assets:** Uso de imagens e som (`star.png`, `starNight.png`, `vozFada`).