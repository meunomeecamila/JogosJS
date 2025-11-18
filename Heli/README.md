# 🚁 Operação de Entrega de Ajuda (Helicopter Drop)

### Simulação de física de queda livre para entrega de suprimentos, desenvolvida com p5.js e Matter.js.

Este projeto simula uma **missão de entrega de ajuda**, onde o jogador controla um helicóptero para posicionar um pacote de suprimentos sobre uma **zona de destino (drop zone)** vermelha e, em seguida, liberá-lo. 

A lógica de movimento do helicóptero e do pacote antes da queda é controlada pelo p5.js, enquanto a **queda livre**, a **colisão** com o solo e o **comportamento físico** do pacote são gerados com precisão usando a biblioteca **Matter.js**. O objetivo é garantir que o pacote caia exatamente dentro da área de destino.

---

## ✨ Características do Jogo

* **Física de Queda Livre:** Utiliza o **Matter.js** para simular a gravidade e o comportamento do pacote após ser liberado.
* **Controle do Helicóptero:** O jogador pode mover o helicóptero (e o pacote acoplado) lateralmente para posicionamento usando as setas do teclado.
* **Zona de Destino:** Uma área demarcada em vermelho (caixas laterais e base) que define o local exato de entrega.
* **Detecção de Colisão:** O pacote colide realisticamente com o solo e com os limites da zona de destino, graças ao Matter.js.
* **Sprites:** Uso de imagens personalizadas (`helicopter.png` e `package.png`) para a representação visual dos objetos.
* **Estados de Movimento:** O pacote inicia estático, fixado ao helicóptero, e é liberado dinamicamente (`isStatic:false`) ao pressionar a tecla correta.

---

## 🕹️ Como Jogar

O objetivo é soltar o pacote de forma que ele caia e repouse dentro da caixa vermelha na parte inferior da tela.

1.  **Movimento Lateral:** Use as setas **Esquerda ($\leftarrow$)** e **Direita ($\rightarrow$)** para mover o helicóptero e o pacote sobre a área de entrega.
2.  **Soltar o Pacote:** Pressione a seta **Para Baixo ($\downarrow$)** para desativar a propriedade estática do pacote, liberando-o em queda livre.
3.  **Entrega Bem-Sucedida:** O jogo termina quando o pacote atinge o solo ou repousa dentro da zona de destino.

---

## ⚙️ Tecnologias Utilizadas

* **JavaScript:** Linguagem principal de programação.
* **Matter.js:** Biblioteca de física 2D, essencial para a simulação de gravidade, colisões e corpos rígidos.
* **p5.js:** Framework de desenho e renderização (criação de sprites, ambiente e loop de jogo).