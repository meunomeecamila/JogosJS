# 🦖 T-Rex Runner (Dino Game)

### Recriação fiel do clássico "Dino Game" do Google Chrome, onde o T-Rex deve correr e saltar sobre obstáculos para pontuar, desenvolvido com p5.js.

Este projeto é uma implementação completa do popular jogo de corrida infinita T-Rex Runner. O jogador controla um **T-Rex** que corre através de um cenário em constante movimento. O objetivo é **pular** sobre os cactos e desviar dos pterodáctilos (embora apenas cactos estejam codificados) pelo maior tempo possível.

O jogo apresenta um **sistema de pontuação** que aumenta continuamente e, crucialmente, utiliza um sistema de **estados de jogo** (`JOGAR` e `ENCERRAR`) para gerenciar as transições entre a jogabilidade ativa e o fim do jogo após uma colisão. 

---

## ✨ Características do Jogo

* **Corrida Infinita:** O solo (`solo`) é um background em loop que se move continuamente para a esquerda, reiniciando sua posição para criar a ilusão de um cenário infinito.
* **Salto e Gravidade:** O T-Rex pula quando a tecla **Espaço** é pressionada, com um efeito de gravidade simulado (aumento gradual do `trex.velocityY`).
* **Dificuldade Crescente:** A velocidade do solo e dos obstáculos aumenta gradualmente conforme a pontuação sobe (`solo.velocityX = -(6 + 3*pontuacao/100)`).
* **Sistema de Pontuação:** A pontuação é calculada com base no tempo de jogo (`getFrameRate()/60`).
* **Estados de Jogo:** O código gerencia as duas fases do jogo:
    * **JOGAR (1):** T-Rex corre, obstáculos e nuvens são gerados, pontuação aumenta.
    * **ENCERRAR (0):** T-Rex para, solo para, objetos são congelados, e as imagens de "Game Over" e "Reiniciar" aparecem.
* **Obstáculos Aleatórios:** Os cactos são gerados aleatoriamente com diferentes sprites (`obstacle1` a `obstacle6`).
* **Reiniciar Jogo:** A função `reset()` é chamada ao clicar no botão de reiniciar (`mousePressedOver(reiniciar)`), restaurando o jogo para o estado `JOGAR`.

---

## 🕹️ Como Jogar

1.  **Iniciar/Pular:** Pressione a tecla **Espaço** para fazer o T-Rex pular sobre os obstáculos.
2.  **Desviar:** Cronometre seus saltos para evitar colidir com os cactos.
3.  **Reiniciar:** Após colidir, clique no botão de **Reiniciar** que aparece na tela.

---

## ⚙️ Tecnologias Utilizadas

* **JavaScript:** Linguagem principal de programação.
* **p5.js (Bibliotecas de Sprites):** Framework principal para:
    * Gerenciamento de sprites (`createSprite`, `addAnimation`, `destroyEach`).
    * Detecção de colisão (`isTouching`).
    * Criação e gerenciamento de grupos de objetos (`new Group()`).
* **Assets:** Uso de múltiplas imagens para o T-Rex, solo, nuvens, cactos, e telas de Fim de Jogo.