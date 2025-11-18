# 🧱 Simulação de Blocos Físicos (Blocks & Gravity)

### Um projeto introdutório que demonstra os fundamentos da física 2D (gravidade e colisões) usando as bibliotecas Matter.js e p5.js.

Este projeto é um *sandbox* simples focado em simular o comportamento de corpos rígidos sob a influência da gravidade. Ele serve como uma excelente demonstração de como inicializar um mundo físico usando o **Matter.js**, adicionar objetos (blocos) e um plano de solo, e observar suas interações.

O código cria dois objetos retangulares (`Box`) que caem sob a gravidade e interagem (colidem e empilham) com o solo (`Ground`) e entre si, reforçando conceitos como **queda livre** e **restrição estática**.

---

## ✨ Características da Simulação

* **Fundamentos de Física 2D:** Demonstra a aplicação da gravidade padrão do Matter.js em corpos dinâmicos.
* **Corpos Rígidos:** Criação de dois objetos retangulares dinâmicos (`box1` e `box2`) que se movem e colidem.
* **Solo Estático:** Um plano de solo (`solo`) que é fixo (`isStatic: true`), atuando como o ponto de colisão final para os blocos.
* **Motor de Simulação:** Utiliza `Engine.update(engine)` no loop principal para calcular o movimento e as interações a cada quadro.

---

## 🕹️ Como Interagir

A simulação é passiva e serve para observação:

1.  **Início:** Ao executar o código, o motor da física é iniciado.
2.  **Observação:** Observe como os blocos caem em diferentes velocidades (devido às suas diferentes posições iniciais) e como eles interagem ao colidir uns com os outros e com o solo.

---

## ⚙️ Tecnologias Utilizadas

* **JavaScript:** Linguagem principal de programação.
* **Matter.js:** A biblioteca de física 2D, utilizada para:
    * Gerenciar o mundo e o motor (`Engine`, `World`).
    * Criar corpos retangulares (`Bodies`).
    * Aplicar a gravidade e processar colisões.
* **p5.js (Implícito):** Framework de desenho e renderização (responsável por criar o canvas, desenhar o fundo e exibir os objetos com `display()`).
