# Game Mata-Mosquito — Arcade Game em JavaScript Vanilla & DOM Engine

[![JavaScript](https://img.shields.io/badge/JavaScript-Vanilla_ES6-F7DF1E?style=flat-square&logo=javascript&logoColor=black)](https://developer.mozilla.org/pt-BR/docs/Web/JavaScript)
[![HTML5](https://img.shields.io/badge/HTML5-Canvas_&_DOM-E34F26?style=flat-square&logo=html5&logoColor=white)](https://developer.mozilla.org/pt-BR/docs/Web/HTML)
[![CSS3](https://img.shields.io/badge/CSS3-Animations_&_Sprite_Transforms-1572B6?style=flat-square&logo=css3&logoColor=white)](https://developer.mozilla.org/pt-BR/docs/Web/CSS)
[![Status](https://img.shields.io/badge/Status-Portfolio_Project-blue?style=flat-square)](#)

Jogo arcade interativo desenvolvido em **JavaScript Vanilla**, fundamentado em manipulação dinâmica do DOM, loops de tempo com `setInterval`, controle de estados de jogo (menu, gameplay, vitória e game over) e lógica matemática para geração de coordenadas espaciais responsivas à resolução da tela.

---

## 🎯 Objetivo

Desenvolver um jogo 2D completo sem o uso de engines pesadas ou bibliotecas externas, demonstrando o uso de JavaScript puro para criação de loops de tempo, detecção de cliques, controle de ciclo de vida de entidades na tela e responsividade dinâmica.

---

## ✨ Mecânicas & Funcionalidades

- **Loop de Criação Dinâmica**: Geração programática de elementos `<img>` no DOM com tempo de vida limitado por tick do timer.
- **Cálculo Espacial Responsivo**: Algoritmo que lê as dimensões da janela em tempo real (`innerWidth` / `innerHeight`) e posiciona os alvos garantindo que não ultrapassem as bordas visíveis.
- **Variação Aleatória de Sprites**:
  - **Tamanhos dinâmicos**: Três escalas visuais distintas (`mosquito1`, `mosquito2`, `mosquito3`).
  - **Orientação (Mirroring)**: Inversão horizontal aleatória via CSS `transform: scaleX(-1)` para dinamismo visual (`ladoA` e `ladoB`).
- **Níveis de Dificuldade**: Seleção no menu inicial transmitida via query string (`window.location.search`):
  - **Normal**: Spawn a cada 1500ms
  - **Difícil**: Spawn a cada 1000ms
  - **Chuck Norris**: Spawn a cada 750ms
- **Sistema de Vidas**: HUD com corações que transitam dinamicamente de cheios para vazios a cada elemento não eliminado a tempo.
- **Condições de Vitória e Derrota**:
  - **Vitória**: Sobreviver à contagem regressiva de 15 segundos (`vitoria.html`).
  - **Derrota**: Esgotar os 3 corações de vida (`fim_de_jogo.html`).

---

## 🧰 Stack Tecnológica

- **JavaScript Vanilla (ES6)**:
  - Temporizadores assíncronos (`setInterval`, `clearInterval`).
  - Manipulação da API DOM (`createElement`, `appendChild`, `remove`, manipulação de estilos e atributos).
  - Funções de aleatoriedade com `Math.random()` e `Math.floor()`.
  - Tratamento de eventos de clique (`onclick`).
- **HTML5**: Telas de menu (`index.html`), palco de jogo (`app.html`), vitória (`vitoria.html`) e game over (`fim_de_jogo.html`).
- **CSS3**: Efeitos visuais, cursores customizados, background responsivo e classes de transformação para dimensionamento de sprites.

---

## 📁 Estrutura do Projeto

```text
Projeto-do-Curso-Desenvolvedor-Web-2022-6/
├── index.html          # Menu principal com seleção de nível
├── app.html            # Palco do jogo e HUD de cronômetro/vidas
├── vitoria.html        # Tela de celebração de vitória
├── fim_de_jogo.html    # Tela de Game Over com opção de reinício
├── jogo.js             # Motor principal do jogo (timers, DOM, regras)
├── estilo.css          # Estilos do jogo, classes de tamanho e orientações
├── imagens/            # Sprites, ícones de corações e cenários
└── README.md           # Documentação técnica do projeto
```

---

## 🚀 Como Jogar

1. Clone o repositório:
   ```bash
   git clone https://github.com/wallacextreme/Projeto-do-Curso-Desenvolvedor-Web-2022-6.git
   ```
2. Abra o arquivo `index.html` em qualquer navegador web moderno.
3. Escolha o nível de dificuldade desejado e clique em **Iniciar Jogo**.

---

## 📌 Status

- **Maturidade**: Projeto de Portfólio / Lógica de Jogos e DOM.
- **Competências demonstradas**: Game loops nativos, manipulação precisa do DOM, responsividade dimensional e algoritmos de aleatoriedade.

---

## 👨‍💻 Autor

Desenvolvido por **[Wallace Soares](https://github.com/wallacextreme)**.