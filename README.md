# Truco Gaúcho

Jogo 2D em pixel art de **truco gaúcho**, ambientado num boteco gaúcho. Usa as mesmas regras do truco espanhol, com o mesmo baralho.

> Status: protótipo das telas iniciais. A mesa de jogo e a lógica do truco ainda serão implementadas.

## O que já existe

- **Tela de abertura** — clique ou Enter/Espaço para continuar
- **Menu principal** — botões *Iniciar* e *Configurações*
- **Modos de jogo** — *1vs1* (local) e *1vsRobo*
- **Configurações** — painel com volume de música/efeitos e dificuldade (ainda sem efeito no jogo)

Os modos de jogo ainda mostram um aviso de "em construção".

## Como rodar

Não precisa instalar nada. Abra o `index.html` direto no navegador, ou suba um servidor local:

```bash
python3 -m http.server 8000
# acesse http://localhost:8000
```

## Estrutura

```
index.html        estrutura das 3 telas
css/style.css     visual, animações e posição dos botões
js/main.js        navegação entre telas, modal e avisos
assets/           artes em pixel art (abertura, menu, modos)
docs/             apresentação da faculdade (.pptx)
```

## Como funcionam os botões

Os botões já estão desenhados dentro das artes. Cada tela é um contêiner com o mesmo `aspect-ratio` da imagem, e `<button>` transparentes são posicionados em porcentagem sobre cada placa de madeira. Assim os cliques continuam alinhados em qualquer tamanho de janela.

## Tecnologias

HTML5, CSS3 e JavaScript puro (sem frameworks). Fonte [Press Start 2P](https://fonts.google.com/specimen/Press+Start+2P) via Google Fonts.

## Próximos passos

1. Distribuição de cartas
2. Cálculo das manilhas
3. Truco / Aumento / Retruco
4. Pontuação e vitória
5. Modo 1vs1 local primeiro; depois 1vsRobo
