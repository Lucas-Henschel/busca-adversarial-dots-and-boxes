# Definição do jogo: Pontos e quadrados

**Acadêmicos**: Ana Caroline Henschel, Christian Alves do Santos, Lucas Gabriel Henschel, León Máximos Ramos e Nicolle Formigari Poncio.

## 1. ⁠Jogo escolhido: Qual jogo o grupo escolheu? Quais são suas regras?

O jogo escolhido foi Pontas e quadrados. Cada jogador na sua rodada, na sua vez, deve marcar uma linha horizontal ou vertical entre dois pontos adjacentes que ainda não estejam conectados.

Se um jogador completar um quadrado, ele marca 1 ponto e recebe o direito de realizar uma nova jogada. Caso não complete nenhum quadrado a vez passa para o adversário.

O jogo termina quando todas as linhas forem preenchidas, sendo declarado vencedor quem conquistar mais quadrados.

## 2. ⁠Estado inicial: Como o jogo começa? Como esse estado pode ser representado?

O jogo começa com um tabuleiro vazio, composto por 6x6 pontos, que permitem a formação de 25 quadrados (5x5).

Computacionalmente, o estado pode ser representado por uma matriz de 11x11, na qual são armazenadas as posiçõs dos pontos, das linhas horizontais e verticais e dos quadrados.

No início do jogo, nenhuma linha está marcada e ambos os jogadores possuem pontuação zero. O estado deve armazenar o jogador responsável pela próxima jogada e a pontuação de cada participante.

## 3. ⁠Jogadores: Quantos jogadores participam? Quem são MAX e MIN?

O jogo possui dois jogadores. O computador seria o jogador MAX, com o objetivo de maximizar sua vantagem na pontuação e o humano seria o jogador MIN, que tenta minimizar essa vantagem.

## 4. ⁠Ações possiveis: Quais ações cada jogador pode executar? existem restrições?

Em cada rodada dos jogadores eles podem marcar uma linha horizontal ou vertical entre dois pontos adjacentes. Porém não é permitido:
- marcar uma linha que já foi marcada;
- marcar linhas diagonais;
- tentar conectar pontos que não estão ligados;
- marcar linhas onde ultrapasse os limites do tabuleiro

O tabuleiro possui 60 linhas possíveis, sendo 30 horizontais e 30 verticais. A cada jogada uma dessas linhas deixa de estar disponível.

# 5. ⁠Função de transição: Como o estado do jogo muda após cada ação?

Caso um jogador marque uma linha e complete um quadrado, ele marca o quadrado e ganha um ponto, podendo jogar novamente.
Caso não complete um quadrado, a vez passa para o outro jogador.

## 6. ⁠Estado terminal: Em quais situações o jogo termina? Como identificar vitória, derrota ou empate?

O jogo termina quando todas as linhas forem marcadas.
Vitória: O jogador que completar mais quadrados vence.
Derrota: O jogador que completar menos quadrados perde.
Não há empate, pois o número de quadrados é ímpar.

## 7. Função de utilidade: Como serão atribuidas pontuações aos resultados do jogo?

Cada quadrado completado vale 1 ponto para o jogador que desenhou a última linha necessária para fechá-lo.

## 8. ⁠Tipo de jogo: O jogo é determinístico ou estocástico? Por quê?

Determinístico, pois não existe aleatoriedade no jogo. Todas as ações possíveis e suas consequências são conhecidas pelos jogadores.
