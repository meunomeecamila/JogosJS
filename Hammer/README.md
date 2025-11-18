# 🔨 Jogo do Martelo (Hammer Game)

### Simulação de física onde o jogador interage com o ambiente usando um Martelo (Hammer) controlável pelo mouse, desenvolvido com Matter.js e p5.js.

Este projeto foca na implementação de um objeto de jogo principal, o **Martelo (Hammer)**. O martelo é um corpo rígido definido pelo **Matter.js** que o jogador pode **controlar diretamente com o mouse**.

O objetivo deste componente é permitir que o jogador utilize o martelo para interagir com outros corpos na simulação (como esmagar objetos, mover pilhas de blocos ou moldar materiais), simulando um ambiente de ferraria ou construção. 

---

## ✨ Características do Componente

* **Controle pelo Mouse:** A posição do martelo (`this.body.position`) é continuamente sincronizada com a posição do cursor do mouse (`mouseX`, `mouseY`), proporcionando um controle intuitivo.
* **Corpo Rígido (Matter.js):** O martelo é definido com alta densidade ($\text{density}: 4$) para garantir que tenha um **impacto significativo** e realista nas colisões com outros objetos.
* **Física Customizada:** O objeto possui atributos físicos ajustados para simular um martelo pesado:
    * **Densidade:** $\text{density} = 4$ (Alto peso).
    * **Fricção:** $\text{friction} = 1.0$ (Maior resistência ao contato).
    * **Restituição (Elasticidade):** $\text{restitution} = 0.5$ (Salto moderado nas colisões).
* **Visualização:** O martelo é renderizado como um retângulo laranja com contorno branco (`stroke('white')` e `fill('orange')`) e sua rotação é gerenciada pelo ângulo físico (`this.body.angle`) do Matter.js.

---

## 🕹️ Como Jogar (Interação com o Martelo)

A interação é baseada no uso do cursor:

1.  **Mover:** Mova o cursor do mouse pela tela. O martelo o seguirá imediatamente, permitindo que você o posicione.
2.  **Interagir:** Colida o martelo com quaisquer outros corpos presentes no mundo (blocos, esferas, etc.) para aplicar força, movê-los ou esmagá-los.

---

## ⚙️ Tecnologias Utilizadas

* **JavaScript:** Linguagem principal.
* **Matter.js:** Biblioteca de física 2D, essencial para definir o martelo como um corpo rígido com propriedades de massa e colisão.
* **p5.js:** Framework de desenho e renderização (responsável por desenhar o martelo e capturar a entrada do mouse).