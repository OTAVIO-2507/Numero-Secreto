<div align="center">

# Jogo do Número Secreto

Jogo de adivinhação no navegador: o jogador tenta descobrir o número secreto entre 1 e 10 recebendo dicas a cada palpite, com feedback por voz sintetizada e contagem de tentativas.

![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=flat-square&logo=html5&logoColor=white)
![CSS3](https://img.shields.io/badge/CSS3-1572B6?style=flat-square&logo=css&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=flat-square&logo=javascript&logoColor=black)

[![Ver projeto](https://img.shields.io/badge/Ver_projeto-3642B5?style=for-the-badge&logo=googlechrome&logoColor=white)](https://otavio-2507.github.io/Numero-Secreto/)
[![Código](https://img.shields.io/badge/C%C3%B3digo-000000?style=for-the-badge&logo=github&logoColor=white)](https://github.com/OTAVIO-2507/Numero-Secreto)

<br>

[![Prévia do projeto](img/preview.jpg)](https://otavio-2507.github.io/Numero-Secreto/)

</div>

## Visão geral

Projeto de lógica de programação com JavaScript: a cada rodada um número aleatório é sorteado e o jogador recebe, além do texto na tela, mensagens faladas (via ResponsiveVoice) indicando se o palpite está acima ou abaixo do número secreto. Ao acertar, o jogo informa o total de tentativas e permite iniciar uma nova partida, sem repetir números já sorteados até esgotar a lista.

## Funcionalidades

- Sorteio de número secreto sem repetição entre partidas consecutivas
- Dicas em tempo real: o palpite está acima ou abaixo do número secreto
- Feedback por voz sintetizada com ResponsiveVoice
- Contagem de tentativas exibida ao vencer
- Botão de nova partida habilitado apenas após o acerto
- Interface responsiva com tipografia temática

## Decisões de projeto

Algumas escolhas que não são óbvias pelo código:

**A lista de sorteados zera ao esgotar o intervalo.** `gerarNumeroAleatorio` guarda os números já usados e chama a si mesma quando repete, para que duas partidas seguidas não tenham o mesmo segredo. Sem o reset ao encher a lista, a partida seguinte à última entraria em recursão infinita procurando um inédito que acabou.

**A fala não é um recurso à parte.** `exibirTextoNaTela` escreve no DOM e sintetiza o mesmo texto na mesma chamada, então tela e áudio não têm como divergir: não existe caminho no código que atualize um sem o outro.

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

