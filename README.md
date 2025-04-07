# Snake Game 🐍

Uma versão moderna do clássico jogo **Snake**, desenvolvida em **Java** com uso de **POO (Programação Orientada a Objetos)** e **Swing/AWT** para renderização gráfica.

## 🎯 Objetivo

O projeto visa exercitar conceitos de programação orientada a objetos, estruturação modular de código e criação de interfaces gráficas em Java.

---

## 🧰 Tecnologias Utilizadas

- **Java 8+** – Linguagem de programação.
- **Swing & AWT** – Bibliotecas padrão para GUI e gráficos 2D.
- **Maven** – Gerenciador de build (estrutura padrão de projeto).

---

## 🗂️ Estrutura do Código

O código está dividido em pacotes para melhor organização:

### Principais Classes:

- [`Game.java`](https://github.com/VimBSD/Snake-Game/blob/main/Snake/src/main/java/snake/Game.java)  
  Classe principal que inicializa o jogo e a janela (`JFrame`).

- [`GamePanel.java`](https://github.com/VimBSD/Snake-Game/blob/main/Snake/src/main/java/snake/GamePanel.java)  
  Estende `JPanel` e representa o canvas do jogo. Aqui ficam os métodos de:
  - Atualização do jogo (`update`)
  - Renderização gráfica (`paintComponent`)
  - Captura de teclado (`KeyAdapter`)

- [`Snake.java`](https://github.com/VimBSD/Snake-Game/blob/main/Snake/src/main/java/snake/Snake.java)  
  Lida com a lógica da cobra:
  - Movimento
  - Crescimento ao comer
  - Detecção de colisões

- [`Food.java`](https://github.com/VimBSD/Snake-Game/blob/main/Snake/src/main/java/snake/Food.java)  
  Representa a comida gerada aleatoriamente no campo.

- [`Direction.java`](https://github.com/VimBSD/Snake-Game/blob/main/Snake/src/main/java/snake/Direction.java)  
  Enum para definir a direção da cobra (CIMA, BAIXO, ESQUERDA, DIREITA).

---

## ▶️ Como Rodar o Projeto

1. Clone o repositório:
   ```bash
   git clone https://github.com/VimBSD/Snake-Game.git
   cd Snake-Game/Snake
   ```

2. Compile e execute com:
   ```bash
   mvn compile
   mvn exec:java -Dexec.mainClass="snake.Game"
   ```

   Ou, manualmente com Java:
   ```bash
   javac -d out src/main/java/snake/*.java
   java -cp out snake.Game
   ```

---
## 📸 Demonstração
![2023-01-24T04:10:06,657838795-03:00](https://user-images.githubusercontent.com/121329916/214249403-828e1c24-94bf-48d8-8113-3ddfb40357e5.png)
![2023-01-24T04:10:20,908841751-03:00](https://user-images.githubusercontent.com/121329916/214249455-ce9f66ea-facf-491f-bfa3-3ad65a57ad64.png)
---

## 🚀 Possíveis Melhorias

- Adicionar placar e tela de game over.
- Incluir som e música.
- Criar níveis com obstáculos.
- Suporte a múltiplos jogadores.

---

## 👤 Autor

[github.com/VimBSD](https://github.com/VimBSD)

---
