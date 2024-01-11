# Modulo38-ebac

**Título: Desenvolvimento Solução de Análise de Dados Eficiente na AWS: Uma Jornada com AWS Lambda, Step Functions e EventBridge**

Introdução:

Olá, comunidade! Hoje, gostaria de compartilhar minha jornada recente explorando as capacidades da AWS para criar uma solução de análise de dados robusta. Neste artigo, detalharei minhas experiências replicando atividades de aulas específicas e abordarei como utilizei AWS Lambda, Step Functions e EventBridge para otimizar o processo.

**AWS Lambda**: 

Na parte 1, embarquei na exploração do AWS Lambda. Seguindo as instruções, repliquei as atividades da aula, que consistiam em extrair dados do site da B3 através de uma API. Dividi essa etapa em duas partes cruciais: extração e transformação.

**Extração**:

Criei um bucket no AWS S3 para armazenar o dado original (bronze).
Desenvolvi uma função AWS Lambda dedicada à extração do dado original, garantindo uma integração eficiente com a API da B3.  

**Transformação**:

Estabeleci outro bucket no AWS S3 para armazenar o dado transformado (silver).
Implementei uma segunda função AWS Lambda para transformar o dado original, preparando-o para análises mais avançadas.
Criada uma função adicional para gerar uma tabela no AWS Athena, apontando para o bucket do dado transformado, facilitando consultas SQL futuras.

**AWS Step Functions**: 

Na parte 2, avancei para a exploração das AWS Step Functions, criando uma state machine com três tarefas, cada uma vinculada a uma função Lambda da etapa anterior.

**Integração de Tasks**:

Integrei as funções Lambda criadas anteriormente em uma state machine eficiente.
As tarefas foram organizadas de forma lógica, garantindo uma execução suave do processo de extração, transformação e preparação para análise de dados.

![](https://github.com/Genesio-Moreira87/Modulo38-ebac/blob/main/images/print_step_functions1.jpg?raw=true)  

**AWS EventBridge**: 

Na parte 3, introduzi AWS EventBridge para automatizar a execução da state machine.

**Criação de Evento**:

Criei um evento personalizado no AWS EventBridge para iniciar automaticamente a state machine desenvolvida na etapa anterior.
Isso proporcionou uma solução automatizada, reduzindo a necessidade de intervenção manual e tornando o processo mais ágil.

**Considerações Finais**:

A combinação dessas tecnologias e serviços AWS permitiu criar uma solução eficaz e escalável para análise de dados.
Em resumo, minha jornada explorando AWS Lambda, Step Functions e EventBridge foi uma experiência enriquecedora, e espero que esta narrativa inspire outros a explorarem as vastas capacidades da AWS para impulsionar suas próprias soluções de análise de dados. Vamos continuar aprendendo, inovando e compartilhando conhecimento!

#AWS #Lambda #StepFunctions #EventBridge #AnáliseDeDados #BancoDeDados #Relatórios #SQLServer #BI #ETL #GitHub #Python





