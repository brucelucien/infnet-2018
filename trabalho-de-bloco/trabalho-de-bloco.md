# 1 INTRODUÇÃO

## 1.1 DOCUMENTO DE VISÃO

## 1.2 APRESENTAÇÃO DO PROJETO

## 1.3 OBJETIVOS GERAIS DO PROJETO

## 1.4 EXPECTATIVAS DO CLIENTE

Criar um formulário eletrônico via web para suportar o processo de avaliação da qualidade do ensino do Infnet.

# 2 REQUISITOS E RISCOS DO PROJETO

## 2.1 FUNCIONAIS

1. Permitir a manutenção de um cadastro de questões do tipo texto com opções de resposta numa escala Likert de cinco graus.

1. Permitir a manutenção de um cadastro de avaliações por usuário com perfil de administrador da solução.

1. Permitir a associação de questões do cadastro de questões com uma determinada avaliação.

1. Garantir que cada avaliação terá um código alfanumérico que a identificará univocamente, criado a critério de um usuário com perfil de administrador da solução.

1. Enviar aos professores o resultado de suas avaliações pelos alunos.

1. Permitir que somente usuários com o papel de administrador do sistema possam definir o período de início de uma determinada avaliação.

1. Enviar e-mails, no momento de início de uma avaliação, a todos os alunos habilitados a participar da avaliação.

1. Permitir a utilização de tags, com tratamento de gênero, e que identificam o aluno, na elaboração do email que será enviado aos alunos.

1. Prever que uma avaliação terá as seguintes informações: objetivo da avaliação, data e hora de início, data e hora de término, matrícula e nome do respondente. identificação do módulo, identificação da turma, identificação do professor e um conjutno de questões copiadas do cadastro de questões.

1. Prever que o texto convidativo para a avaliação seja editável.

1. Imprimir a avaliação por usuários com perfil de administrador.

1. Gerar planílha com o resultado das avaliações.

## 2.2 NÃO FUNCIONAIS

1. Garantir que o formulário web tenha o mesmo layout do formulário de papel utilizado pela instituição.

1. Editar, usando algum editor *rich text*, o código HTML que será enviado no e-mail disparado aos alunos que avaliarão a qualidade do ensino.

1. Permitir que o usuário role verticalmente o formulário eletrônico quando há uma quantidade de questões que ultrapassa o tamanho da tela do usuário. 

1. Evitar a exibição de barras de rolagem horizontais na exibição do formulário eletrônico.

1. Incluir o endereço do link para o questionário no e-mail enviado aos alunos que responderão a avaliação.

1. Fechar automaticamente o formulário de avaliação dois dias úteis após a data de término do módulo.

1. Garantir a segurança de acesso ao questionário, que deve ter acesso autenticado.

1.  Garantir que somente usuários com perfil de administrador possão alterar o texto convidativo enviado por e-mail aos alunos que participarão da avaliação.

1. Garantir que o formulário seja apresentado inicialmente ao aluno com todas as opções desmarcadas.

1. Ter desempenho suficiente para, no mínimo, 1000 alunos matriculados regularmente.

1. Dificultar a impressão da avaliação pelos alunos.

1. Garantir a execução nos browser Mozilla Firefox e Google Chrome.

1. Gerar a planílha com o resultado das avaliações no formato CSV, nomeado como CODIGODAAVALIACAO_MATRICULADOALUNO.

## 2.3 REGRAS DE NEGÓCIO

1. Professores não podem utilizar o sistema.
 
1. Não deve existir preferência de resposta entre as alternativas de uma questão.
 
1. O período de avaliação deve ser automaticamente aberto a partir do momento programado para seu início.

1. Somente os alunos que cursaram um determinado módulo podem responder as avaliações.

1. Normalmente o período de avaliação é aberto no início da última semana do respectivo módulo.

1. Planilhas com os resultados das avaliações são utilizadas pela secretaria para encaminhar as avaliações ao cooordenador de cada curso.

1. Os coordenadores de curso apresentam os resultados das avaliações em reunião pessoal com cada professor.

## 2.4 RISCOS DO PROJETO

|Risco|Causa|Probabilidade|Ação|
|-|-|-|-|
|Projeto deixar de ser relevante à instituição.|Aquisição da instituição por outra empresa.|Baixa|Montar apresentação demonstrando a importância do projeto.|
|Funcionários podem não cooperar com o projeto.|Medo de que o software torne obsoletos seus cargos.|Baixa|Entregas rápidas, com sprints curtos, apresentando aos funcionários o software produzido de forma que possam se familiarizar com ele durante o desenvolvimento projeto e reconhecer sua importância por si mesmos.|
|Baixa produtividade dos desenvolvedores.|Alta rotatividade de desenvolvedores no projeto.|Média|Tornar os cargos da equipe atrativos no que tange a salários, vantagens e ambiente organizacional.|
|Atraso nas datas de entrega definidas.|Erro de estimativa quanto à produtividade da equipe em relação ao tamanho do projeto.|Alta|Medição utilizando pontos de função ou estimativa no formato ágil utilizando planning poker e acompanhamento constante das métricas e dos marcos definidos no projeto.|

# 3 MÉTRICAS DE PROJETO

## 3.1 ESTIMATIVA

### 3.1.1 TAMANHO

117 pontos de função calculados com base na planílha de contagem.

### 3.1.2 PRAZO

2 meses.

Calculamos 48,75 dias úteis com base na divisão da quantidade de dias necessários para a realização do projeto (195 dias, no caso) distribuídos entre quatro pessoas, que é a quantidade de recursos disponíveis para o projeto.

A quantidade de 195 dias é o resultado da divisão da quantidade de horas previstas para a realização do projeto (1.170 horas = 117 PF * 10 h/PF) considerando uma jornada de trabalho diária de 6 horas.

### 3.1.3 ESFORÇO



### 3.1.4 EQUIPE

4 pessoas considerando os 4 componentes do grupo.

### 3.1.5 CUSTO

O custo total do projeto é de R$ 93,600 considerando o custo de R$ 80,00 por hora trabalhada e a quantidade estimada de horas para o projeto (1.170 horas).

### 3.1.6 RECURSOS COMPUTACIONAIS CRÍTICOS

# 4 REFERÊNCIAS BIBLIOGRÁFICAS

# 5 ANEXOS

## 5.1 CASOS DE USO

## 5.2 PLANILHA DE CONTAGEM DE PONTOS DE FUNÇÃO

### 5.2.1 IDENTIFICAÇÃO 

### 5.2.2 FATOR DE AJUSTE

### 5.2.3 SUMÁRIO DE APURAÇÃO DOS PONTOS DE FUNÇÃO NÃO AJUSTADOS
