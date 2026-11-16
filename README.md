Objetivo do Jogo: Controlar o Pac-Man pelo labirinto utilizando as setas direcionais (ou teclas W, A, S, D) para coletar todas as pastilhas sem ser capturado pelos fantasmas.

-> Regras e Pontuação:

* Pastilha comum: 10 pontos.

* Pastilha de poder (cantos do mapa): 50 pontos e deixa os fantasmas vulneráveis (azul-ciano) temporariamente.

* Capturar fantasma vulnerável: 200 pontos.

* Condição de Vitória: Coletar todas as pastilhas do labirinto.

* Condição de Derrota: Perder as 3 vidas ao colidir com fantasmas ativos.

-> Arquitetura Orientada a Objetos:

* Herança e Polimorfismo: A classe abstrata Entidade define atributos e comportamentos comuns (posição, hitbox e detecção de colisão com paredes), sendo estendida por Jogador e Fantasma, que sobrescrevem atualizar() e desenhar().

* Encapsulamento: O estado do mapa e das pontuações fica protegido na classe Labirinto, acessado apenas por métodos controlados.

* Eventos e Interface Gráfica: GamePanel utiliza JPanel, Graphics2D, KeyAdapter (eventos de teclado) e javax.swing.Timer (atualização contínua a 60 FPS) dentro de um JFrame.
