# Jogo do Número Secreto

Jogo de adivinhação no navegador: o jogador tenta descobrir o número secreto entre 1 e 10 recebendo dicas a cada palpite, com feedback por voz sintetizada e contagem de tentativas.

![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white)
![CSS3](https://img.shields.io/badge/CSS3-1572B6?style=for-the-badge&logo=css&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black)

[![Demonstração online](https://img.shields.io/badge/demonstra%C3%A7%C3%A3o-online-2EA44F?style=for-the-badge)](https://otavio-2507.github.io/Numero-Secreto/)

## Visão geral

Projeto de lógica de programação com JavaScript: a cada rodada um número aleatório é sorteado e o jogador recebe, além do texto na tela, mensagens faladas (via ResponsiveVoice) indicando se o palpite está acima ou abaixo do número secreto. Ao acertar, o jogo informa o total de tentativas e permite iniciar uma nova partida, sem repetir números já sorteados até esgotar a lista.

## Funcionalidades

- Sorteio de número secreto sem repetição entre partidas consecutivas
- Dicas em tempo real: o palpite está acima ou abaixo do número secreto
- Feedback por voz sintetizada com ResponsiveVoice
- Contagem de tentativas exibida ao vencer
- Botão de nova partida habilitado apenas após o acerto
- Interface responsiva com tipografia temática

## Tecnologias

| Tecnologia | Aplicação no projeto |
| --- | --- |
| JavaScript (ES6+) | Sorteio, comparação de palpites e controle de estado |
| HTML5 | Estrutura da interface do jogo |
| CSS3 | Estilização e responsividade |
| ResponsiveVoice | Sintetização de voz para as mensagens do jogo |
| Google Fonts | Tipografia (Chakra Petch, Inter) |

## Como executar

```bash
git clone https://github.com/OTAVIO-2507/Numero-Secreto.git
cd Numero-Secreto
```

Abra o arquivo `index.html` no navegador. O jogo é totalmente client-side.

## Estrutura do projeto

```
Numero-Secreto/
├── index.html          Interface do jogo
├── app.js              Lógica do sorteio e das tentativas
├── style.css           Estilos da página
└── img/                Imagens de fundo e ilustração
```

## Autor

**Otávio Oliveira** — Desenvolvedor Full Stack

[GitHub](https://github.com/OTAVIO-2507) · [Portfólio](https://otavio-2507.github.io/Portifolio-v2/) · [E-mail](mailto:56otavio@gmail.com)
