# Beetle Driver - Motorista de fusca

## Dupla: Iago Carvalho Santana e Leo Kenzo Masago

 ## 1. Visão Geral:
Nós escolhemos um tema de um jogo com mecânicas de corrida infinita desenvolvido no Unity. em Beetle Driver, você assume o papel de um habilidoso motorista em fuga, conduzindo um fusca em alta velocidade enquanto é perseguido por um carro de polícia determinado a capturá-lo. Enquanto foge, desvie de carros que se movem rapidamente pela avenida. O objetivo é percorrer e coletar uma espeficia quantidade de moedas sem colidir com outros carros da avenida e sem ser parado pela policia.

 ## 2. Mecânicas Principais:

*2.1. Controle do Carro:*
O jogador pode controlar o carro através das teclas de setas (esquerda e direita) do teclado. Para implementar esse controle, será utilizado o sistema de input do Unity, com o uso da função `Input.GetAxis` para detectar a movimentação horizontal do carro.

*2.2. Geração da Avenida:*
A geração da avenida será feita usando um prefabs, criando segmentos "infinitos" da estrada.

*2.3. Carros Inimigos:*
A geração de carros inimigos será controlada por um sistema randomizado para garantir o desempenho e evitar instanciar e destruir objetos repetidamente. Os carros inimigos serão controlados por um sistema para definir caminhos e evitar colisões.

*2.4. Coleta de Moedas:*
Moedas serão espalhadas ao longo da avenida, e o jogador deverá coletá-las para aumentar sua pontuação. A detecção de coleta de moedas será feita através de colisores e tags especificas no script do jogador. Cada moeda coletada acrescentará um valor específico à pontuação total.

*2.5. Perseguição Policial:*
A perseguição policial será acionada por um evento de progressão, como tempo decorrido. Os carros de polícia serão instanciados no cenário e se movimentarão usando um sistema de seguir o jogador.

 ## 3. Progressão do Jogo:
- O jogo começará com o carro do jogador na avenida, e carros inimigos começarão a ser gerados à frente do jogador.
- O jogador ganhará pontos pela quantidade de moedas coletadas.
- Ao atingir uma quantidade especifica de moedas, o jogador passará para proxima fase

 ## 4. Pontuação:
- Coleta de Moedas: Cada moeda coletada adiciona um valor específico à pontuação total.

 ## 5. Condições de Game Over:
- Colisão: Se o carro do jogador colidir com qualquer outro carro na avenida, o jogo acaba.
- Captura Policial: Se a polícia colidir com o carro do jogador, o jogo termina.

 ## 6. Visual das cenas e Áudio:
- Cena 1: Um Menu simples com botões de iniciar e sair.
- Cena 2: O jogo apresentará uma paisagem urbana neon com modelos de carros brasileiros. O jogador avançará para a próxima fase após coletar uma certa quantidade de moedas.
- Cena 3: A última cena será em uma praia brasileira com paisagens alegres e também modelos de carros brasileiros. O jogador terminará após coletar uma certa quantidade de moedas.
- Áudio: Música de fundo syntwave e efeitos sonoros para movimento do carro, colisões, sons de coleta de moedas e sirenes da polícia.

 ## Aplicativo Mobile :
 O aplicativo será um guia do jogo. Contendo as dicas de jogablidade e explicações para jogar.
 Iremos utilizar ilustrações do jogo com os elementos de ImageView e ListView.
 Para navegar entre as telas pensamos em utilizar Buttons e ImageButtons.
 E para organizar os conteúdos na tela utilizaremos a ScrollView.
