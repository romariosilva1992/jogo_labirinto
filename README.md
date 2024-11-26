# jogo_labirinto

E aí, galera! Vou explicar pra vocês o arquivo LABIRINTO.html que eu criei pro nosso projeto. É um joguinho bem maneiro de labirinto que a gente tá desenvolvendo. Vamos dar uma olhada nas partes principais:

## Estrutura Básica

O arquivo é um HTML simples, mas com bastante coisa legal dentro. A gente tá usando JavaScript pra fazer a mágica acontecer.

## Estilo do Jogo

A gente definiu um estilo bem básico direto no HTML. O corpo da página tá com fundo preto, e a gente tá usando a fonte monospace. Isso dá aquele ar de jogo retrô, saca?

## Canvas do Jogo

O coração do jogo é um elemento `<canvas>`. É nele que a gente vai desenhar todo o labirinto e o jogador. O tamanho tá definido como 400x400 pixels, o que dá um quadrado perfeito pro nosso labirinto.

## Instruções

Logo abaixo do canvas, tem uma mensagem com as instruções: "Use W,A,S,D to move | Find the exit!". Bem direto ao ponto, né? W pra cima, S pra baixo, A pra esquerda e D pra direita. O objetivo é achar a saída do labirinto.

## JavaScript

Agora vem a parte mais legal! Todo o código do jogo tá em JavaScript. Vou explicar as partes principais:

1. **Definição do Labirinto**: A gente tem uma matriz que representa o labirinto. 0 são os caminhos livres, 1 são as paredes.

2. **Posição do Jogador**: O jogador começa na posição [0, 0], que é o canto superior esquerdo.

3. **Funções Principais**:
   - `drawMaze()`: Desenha o labirinto no canvas.
   - `drawPlayer()`: Desenha o jogador (um quadradinho vermelho).
   - `movePlayer()`: Controla o movimento do jogador baseado nas teclas pressionadas.
   - `checkWin()`: Verifica se o jogador chegou na saída.

4. **Controles**: A gente tá usando um event listener pra capturar as teclas pressionadas e mover o jogador.

5. **Loop do Jogo**: Tem uma função `gameLoop()` que roda continuamente, atualizando a posição do jogador e redesenhando tudo.

## Funcionamento

Quando você abre a página, o jogo já começa. Você controla um quadradinho vermelho e tem que navegar pelo labirinto até achar a saída. As paredes são pretas e os caminhos são brancos. Se você chegar no canto inferior direito, você ganha!

## Próximos Passos

Por enquanto, é um jogo bem simples, mas dá pra fazer um monte de coisas legais ainda:
- Adicionar níveis diferentes
- Colocar um timer
- Criar obstáculos móveis
- Implementar um sistema de pontuação

E aí, o que vocês acham? Tô empolgado pra expandir esse joguinho! Se tiverem ideias pra melhorar ou adicionar features, é só falar!
