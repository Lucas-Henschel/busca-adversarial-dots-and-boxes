# Definição do jogo: Pontas e quadrados

**Acadêmicos**: Ana Caroline Henschel, Christian Alves do Santos, Lucas Gabriel Henschel, León Máximos Ramos e Nicolle Formigari Poncio.

## 1. ⁠Jogo escolhido: Qual jogo o grupo escolheu? Quais são suas regras?

Pontas e quadrados. Cada jogador, na sua vez, deve marcar uma linha horizontal entre dois pontos adjacentes.
Se um jogador completar um quadrado, ele marca o quadrado e ganha um ponto, podendo jogar novamente.
O jogo termina quando todas as linhas foram marcadas. O jogador que marcar mais quadrados vence.

## 2. ⁠Estado inicial: Como o jogo começa? Como esse estado pode ser representado?

O jogo começa com um tabuleiro vazio, composto por 11x11 pontos, onde os jogadores podem marcar linhas entre pontos adjacentes (na horizontal e vertical)
O estado do jogo pode ser representado por uma matriz ou lista que indica quais linhas foram marcadas e quais quadrados foram completados.

## 3. ⁠Jogadores: Quantos jogadores participam? Quem são MAX e MIN?

Dois jogadores. O computador seria o jogador MAX e o humano seria o jogador MIN.

## 4. ⁠Ações possiveis: Quais ações cada jogador pode executar? existem restrições?

Marcar uma linha entre dois pontos adjacentes. Não é permitido marcar uma linha que já foi marcada.

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
