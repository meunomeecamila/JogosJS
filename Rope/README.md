# 🔴 Pêndulo de Newton (Newton's Cradle Simulation)

### Uma simulação interativa do clássico Pêndulo de Newton, demonstrando princípios de conservação de momento e energia, desenvolvida com JavaScript e Matter.js.

Este projeto recria o famoso **Pêndulo de Newton**, um dispositivo que ilustra de forma fascinante as leis da física. Ao interagir com as **esferas (bobs)**, você pode observar como o **momento linear** é transferido através delas, resultando no movimento da última esfera. 

[Image of Newton's Cradle]


Toda a lógica física é construída com **Matter.js**, permitindo colisões realistas, conservação de energia (em um mundo simulado) e movimento pendular preciso.

---

## ✨ Características da Simulação

* **Física Realista:** Utiliza o **Matter.js** para modelar com precisão o movimento pendular e as colisões entre as esferas.
    * Módulos chave utilizados: `Engine`, `World`, `Bodies`, `Constraint`.
* **Múltiplas Esferas:** Simulação padrão com **5 esferas** suspensas.
* **Interação por Teclado:** Permite iniciar o movimento aplicando uma força à primeira esfera (**bob1**) usando a tecla **Seta Para Cima** ($\uparrow$).
* **Modelo de Restrição:** As cordas (**ropes**) são implementadas usando o módulo **Constraint** do Matter.js para manter as esferas suspensas.

---

## 🕹️ Como Interagir

A interação é baseada em aplicar uma força inicial para observar o fenômeno físico.

1.  **Execute a Simulação:** Abra o arquivo `index.html` (ou o arquivo principal) em um navegador web.
2.  **Aplique a Força:** Pressione a tecla **Seta Para Cima** ($\uparrow$).
3.  **Observe:** A primeira esfera será lançada contra as outras, e a última esfera se moverá devido à transferência de **momento linear**.

---

## ⚙️ Tecnologias Utilizadas

* **JavaScript:** Linguagem principal de programação.
* **Matter.js:** Biblioteca de física 2D para:
    * Cálculo de colisões e gravidade.
    * Criação de corpos rígidos (`Bodies`).
    * Definição de restrições (`Constraint`) para as cordas.
* **p5.js:** Framework de desenho e renderização (implícito pelo uso de funções como `createCanvas`, `background` e `draw`).

---

## 🧠 Conceitos de Física (Bônus)

O Pêndulo de Newton é uma excelente demonstração das leis de conservação:

* **Conservação do Momento Linear:** O momento total (produto de massa e velocidade, $m \cdot v$) do sistema permanece constante. A colisão transfere esse momento da esfera inicial para a esfera final.
* **Conservação de Energia:** A energia total do sistema (a soma de energia cinética e potencial) permanece constante. A energia cinética da primeira esfera é convertida em energia potencial gravitacional na última esfera que se eleva.