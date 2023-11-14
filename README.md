# trabalho---ArqComp
Desenvolver um simulador que implementa o algoritmo de escalonamento de processos, usando a estratégia de seleção Round Robin (ou Circular) com Feedback.

1. Objetivo do Trabalho
Estimular a capacidade do aluno de trabalhar em equipe para organizar, projetar e desenvolver
soluções para problemas formulados que envolvam o estudo e o conhecimento sobre
gerenciamentos do sistema operacional.
2. Escopo do Trabalho
 Desenvolver um simulador que implementa o algoritmo de escalonamento de processos, usando
a estratégia de seleção Round Robin (ou Circular) com Feedback.
 Preparar um relatório contendo uma descrição sobre os objetivos do trabalho, as premissas
consideradas no desenvolvimento do escalonador e a saída da execução do simulador.
 Os trabalhos devem ser feitos exclusivamente em C.
 As avaliações sobre o funcionamento dos simuladores serão feitas em horário marcado.
3. Equipes de Trabalho
As equipes devem ser formadas com, no máximo, 3 (três) alunos.
4. Prazo de Entrega do Trabalho
Os materiais (código e relatório) devem ser postados no GDrive, pasta “Trabalhos de ICP246 2023-2”
(link:
https://docs.google.com/spreadsheets/d/1Ckd1f4jPEfHOcoye7UWpt6PQKJ0rVqL2JY0xk6SPkrw/edit
#gid=0) até às 23:59 do dia 28/11/2023, com o título “Trabalho 2 de ICP246 – 2023-2 - Grupo X”,
onde X é o número do grupo, conforme descrito na planilha “Grupos Trab 2 - ICP246 – 2023-2”. As
apresentações serão realizadas nos dias 30/11/2023, 04/12/2023 e 06/12/2023, no horário da aula,
em ordem aleatória e previamente disponibilizada no mural do Classroom.
Caso seja necessário, a apresentação dos grupos restantes será realizada em data posterior.
5. Penalidades
Caso o grupo atrase a entrega do trabalho seu grau final sofrerá um decréscimo na razão de 0,5
pontos por dia de atraso.
6. Avaliação
Serão considerados os seguintes aspectos na avaliação do trabalho:
 Execução correta do simulador durante a apresentação - máximo de 10 minutos (3,5 pontos);
 Relatório contendo, minimamente, as premissas do trabalho, a saída do simulador e as
referências utilizadas (3,5 pontos);
 Entrega pontualmente efetuada no dia estipulado (1 ponto);

 Conhecimento utilizado no desenvolvimento do trabalho e distribuição das tarefas entre os
participantes do grupo (2 pontos).

7. Premissas a serem definidas pelo grupo para o desenvolvimento do simulador
 Limite máximo de processos criados;
 O valor da fatia de tempo dada aos processos em execução;
 Tempos de serviço e de I/O aleatórios para cada processo criado;
 Tempos de duração de cada tipo de I/O (disco, fita magnética e impressora);
 Gerência de Processos
o Definição do PID de cada processo,
o Informações do PCB (contexto de software – prioridade, PID, PPID, status);
o Escalonador (pelo menos 3 filas, sendo uma fila de alta e uma de baixa prioridade
para execução na CPU, e 1 fila de I/O, que pode ser implementada com filas
diferentes para cada tipo de dispositivo);

 Tipos de I/O
o Disco – retorna para a fila de baixa prioridade;
o Fita magnética - retorna para a fila de alta prioridade;
o Impressora - retorna para a fila de alta prioridade;
 Ordem de entrada na fila de prontos
o Processos novos - entram na fila de alta prioridade;
o Processos que retornam de I/O – dependente do tipo de I/O solicitado;
o Processos que sofreram preempção – retornam na fila de baixa prioridade.
OBS: As premissas estabelecidas pelo grupo devem estar explícitas no relatório.
