## Medieval Battle <img align="center" alt="Java" height="30" width="40" src="https://raw.githubusercontent.com/devicons/devicon/master/icons/java/java-original.svg">
Medieval Battle, é um jogo de batalha por turnos desenvolvido em Java como parte do Projeto de Conclusão da disciplina "Fundamentos de Desenvolvimento em JAVA". O jogo simula batalhas entre heróis escolhidos pelos jogadores e monstros selecionados aleatoriamente.

## Descrição do Projeto
O projeto consiste em dois programas:

 - 1 Programa Principal: Realiza a simulação de batalhas entre um herói e um monstro.
 - 2 Programa de Relatórios: Lê os logs gerados pelas batalhas e apresenta um relatório detalhado com estatísticas.

## Funcionalidades
Programa Principal
 - Inicialização: O jogo começa solicitando o nickname do jogador e a classe de herói desejada.
 - Simulação de Batalha:
 - Cálculo de Iniciativa: Determinado por um dado de 10 faces (1d10) somado ao fator de agilidade.
 - Ataque e Defesa: Calculados com base em dados, agilidade, força e defesa.
 - Cálculo de Dano: Baseado em um dado e nos pontos de força do personagem.
 - Finalização da Batalha: A batalha termina quando os pontos de vida de um dos personagens chegam a zero.

## Gravação de Log:
Ao final de cada batalha, gera um arquivo CSV com o formato nicknameDoJogador.csv na pasta temp contendo informações da batalha, como data, herói, resultado, monstro enfrentado e quantidade de rodadas.

## Programa de Relatórios
Geração de Relatórios:
 - Solicita o nickname do jogador e busca o arquivo correspondente na pasta temp.
 - Gera estatísticas como herói mais jogado, monstro mais enfrentado, e total de pontos acumulados.
 - Calcula a pontuação de cada batalha com base na fórmula: 100 - quantidadeDeRodadas.
 - Tecnologias Utilizadas
 - Java: Linguagem de programação principal.
 - API de Streams do Java 8: Utilizada para manipulação e processamento dos dados do arquivo CSV.
 - Polimorfismo e Interfaces: Para implementar diferentes comportamentos de personagens.
 - Tratamento de Exceções: Aplicado especialmente para entrada de dados.

## Estrutura do Projeto
 - Classe de Personagem: Classe abstrata ou interface para representar heróis e monstros, com métodos polimórficos para cálculo de dano, ataque e defesa.
 - Classe de Batalha: Responsável por simular a batalha, calcular iniciativas, ataques e definir o vencedor.
 - Classe de Relatório: Processa os dados dos arquivos CSV e gera estatísticas.
