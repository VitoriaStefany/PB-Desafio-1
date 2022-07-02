<h1 align="center">Desafio #001 PB-NODE.JS</h1>

### 1. Para que serve o método Scrum?
> Para fazer o gerenciamento de projetos complexos, em que os requisitos não são totalmente definidos. Transforma um projeto grande e complexo em tarefas bem definidas de forma priorizada. E juda o time a focar e desenvolver as tarefas dentro de determinado tempo previamente planejado (Sprint), de forma que venha agregar valor ao produto até o final da Sprint. Priorizando a melhoria contínua, com reuniões que ajudam a identificar eventuais impedimentos, de forma que ajude o desenvolvimento fluir.

### 2. Como funciona o método Scrum? 
> Todo o projeto é planejado para ser realizado em Sprints que são um série de iterações e incrementos. A Sprint é composta por time-boxes, que são, no sentido literal, caixas de tempo limitada e inflexível. Ou seja, é o tempo em que o time usará para agregar valor para o produto no final da Sprint. Geralmente a Sprint pode durar de 3 (três) dias até 4 (quatro) semanas, sendo mais comum a Sprint de 2 (duas) semanas. 

> É essencial entender, que a equipe de um projeto trata-se de um time, onde não há hierarquia e o sucesso do projeto, é uma responsabilidade igualmente distribuída para todos os integrantes do time, por mais que estes desempenhem papéis diferentes. Os papéis existentes em um time Scrum são o do Product Owner, do Scrum Master e da equipe de desenvolvedores (ou Dev Team). 

> O time levará em consideração o Product Backlog do Product Owner, que é a lista de requisitos priorizada que o P.O. produziu com base em seu entendimento das necessidades do cliente para agregar valor ao produto. O P.O. apresentará as histórias (itens) do Product Backlog, para o time na _Planning Meentig_, que é primeira time-box da Sprint. Todo o time discute o que entrará na Sprint Backlog que funciona como roteiro, ou pelo menos contém o topo da lista do Product Backlog, com as tarefas da próxima Sprint.

> #### FASES/TIME-BOXES DA SPRINT
> 1. **_Plannig Meeting_**: Reunião de planejamento com todo o time Scrum. Onde serão definidas as tarefas da próxima Sprint, tomando como o base o Product Backlog do P.O., que traz as histórias que serão transformadas em tarefas.

 > 2. **Desenvolvimento**: Período de foco para executar o que foi proposto na _Planning Meenting_.
 >> - **Daily Scrum**: Durante o processo de desenvolvimento, são realizadas reuniões diárias com duração de até 15 minutos, em que todo o time participa, e onde são levantadas as seguintes questões para o time de desenvolvimento:
 >>> - O que fiz?
 >>> - O que pretendo fazer?
 >>> - Quais os impedimentos?

> 3. **_Review Meenting_**: Reunião em que participa todo o time Scrum, o cliente e/ou usuário. São apresentados todos os incrementos que foram feitos durante o desenvolvimento da Sprint. Essa time-box não é maior que 2,5% do tempo total da Sprint.

> 4. **_Retrospective_**: Reunião de melhoria contínua com todo o time Scrum. Onde são levantados os pontos positivos e os pontos negativos da Sprint e verificar onde é necessário melhorar para a próxima Sprint. É o última time-box da Sprint.

### 3. O que é Git? 
> É um sistema de controle de versões de projetos. Ou seja, permite que uma pessoa, um grupo, equipe ou time, trabalhe em um projeto armazenando as versões, modificações e o histórico das atualizações do projeto. De forma que todos têm acesso a versão mais atualizada e de todo o histórico.

### 4. O que é um scrum Product Owner? 
> O Product Owner é o representante do cliente. Ele entende as necessidades, as prioridades e reconhece o que agrega valor ao produto. É responsável por produzir e manter atualizada a lista de requisitos priorizada ou Product Backlog, que contém histórias de onde saíram as tarefas para a compor a _Sprint Backlog_, na ordem de prioridade, que serão realizadas na próxima Sprint. Durante o processo, ele deve tirar as dúvidas do time acerca do produto, ou indicar quem pode sanar a dúvida.

### 5. Qual o comando para criação de um novo repositório no Git? 
> Comando para executar dentro do local onde será repositório: `$ git init`

### 6. O que é o HTTP?
> O Hiper Text Transfer Protocol ou Protocolo de Transferência de Hipertexto, trata-se de um protocolo de comunicação que é um conjunto de regras, para que seja possível a comunicação entre cliente e servidor na web. Ou seja, é o protocolo HTTP que define as regras de comunicação de requisição e resposta na internet. É o protocolo mais importante da internet!

### 7. Como funciona o HTTP? 
> Na arquitetura Cliente-Servidor, através dos protocolos (conjunto de regras bem definidas), uma aplicação web (cliente), por exemplo, faz requisições (_HTTP REQUEST_) de um site (servidor) com informações e com o método indicando a ação que deseja receber. O servidor por sua vez envia a resposta (_HTTP RESPONSE_) da requisição, que pode ser uma página web, como exemplo. A comunicação sempre será iniciada pelo cliente, e  nessa comunicação são constituídas as URLs. Cada requisição realizada é única, ou seja, uma requisição não tem conhecimento da requisição anterior, é uma característica do HTTP chamada _STATELESS_. Então, para que não seja necessário refazer a validação de usuário em uma em determinada página que necessita de credenciais para login, por exemplo, o servidor envia uma identificação para o navegador, que guarda em arquivos de cookies, e a utiliza durante aquela sessão.

> Os métodos de requisição, que é a ação esperada pelo navegador (cliente), podem ser apenas para receber informações enviando parâmetros pela URL como método `GET`, criar algo novo no servidor ou apenas esconder os parâmetros como método `POST`. Existem ainda outros três métodos: o método `PUT` para fazer atualização, o método `PATCH` para modificar de forma parcial e o método `DELETE` para excluir um recurso. 
Os códigos de status, que recebemos como resposta das requisições, servem para identificar se a requisição teve sucesso ou não. Ou seja, dependendo da resposta, podemos receber um _STATUS CODE_ diferente. Por exemplo, ao fazer uma requisição, o navegador recebe o _STATUS CODE_ `200`, isso significa que a requisição teve sucesso e a página foi exibida sem impedimentos. Porém se o _STATUS CODE_ for `404`, significa que o cliente fez uma requisição inválida e o servidor não encontrou o recurso requisitado. Os _STATUS CODE_ mais comuns são da "família" `2xx` que indica sucesso na resposta da requisição, `3xx` de mensagens de redirecionamento, `4xx` requisição inválida pelo cliente e `5xx` que indica erro interno do servidor.

### 8. Com o Git Você pode propor mudanças (adicioná-las ao Index) usando um comando. Qual é esse comando? 
> - Para apenas adicionar apenas um arquivo do diretório: `$ git add <nomedoarquivo>`
> - Para adicionar todos os arquivos do diretório: `$ git add .`
> - E um _commit_ para confirmação da alteração e incluir uma mensagem: `$ git commit -m "Mensagem referente a mudança."` 

### 9. O que é a Branch master e para que serve? 
> É o _Branch master_ é o _Branch_ principal ou padrão. Quando é criado um novo repositório, o mesmo inicia na _Branch master_. Nele contém todo o projeto, e a partir dele são criadas as demais _Branches_ (ramificações).

### 10. Quais são os comandos usados para atualizar um repositório local e fazer merge de um outro branch ao seu branch ativo? 
> `$ git murge <nomedabranch>` Pressione "ENTER".
Em seguida é possível fazer alteração no _commit_. Em seguida pressione "x: + ENTER".
> Também é possível executar o _rebase_: '$ git rebase <nomedabranch>'

### 11. Qual a diferença entre git e github? 
> Enquanto o Git é o software ou sistema de controle de versão. O Github é uma plataforma que utiliza o Git para compartilhar, com outras pessoas, os projetos. Onde é possível exibir o histórico, as versões, e as atualizações do projeto. Também é possível adicionar colaboradores que trabalham no mesmo projeto. E em cada perfil, também é possível armazenar, de forma pública ou privada, todos os projetos em que o usuário trabalha ou está inserido.

### 12. Quais os dois verbos http que podemos utiizar para realizar um update? Explique a diferença entre eles. 
> `PUT` e o `POST`. A diferença é que o `POST` pode ter efeitos adicionais se usado repetidamente, enquanto que o `PUT` pode ser chamado sucessivamente que terá o mesmo efeito. 

### 13. Qual o status code que pode ser usado na criação de um novo usuário? 
> `201 - CREATED`

### 14. Quais são os três status code que podem ser utilizados para realizar o delete? 
> Quando o método _DELETE_ é aplicado com sucesso:
>`202 - ACCEPTED`
>`204 - NO CONTENT`
>`200 - OK`

### 15. Exemplifique para que serve os metódos http 1xx, 2xx, 3xx, 4xx e 5xx. De uma forma macro (geral)!
> * 1xx: Respostas informativas. 
>  Ex.: `101 - CONTINUE`: Resposta provisória. Obteve sucesso e pode continuar ou ignorar.
> * 2xx: Respostas de sucesso. Onde é entregue o que foi requisitado. 
>  Ex.: `200 - OK`: Requisição obteve sucesso!
> * 3xx: Mensagens de redirecionamento. 
  Ex.: `301 - MOVED PERMANENTLY` - A página sempre foi redirecionada para um URL indicado pelo cabeçalho.
> * 4xx: Respostas de erro do cliente. 
  Ex.: `404 - NOT FOUND`: Servidor não encontrou recurso.
> * 5xx*: Resposta de erro do servidor. Quando há um problema interno do servidor. 
  Ex:. `500 - INTERNAL SERVER ERROR` - Erro interno do servidor.

### 16. Conta pra gente como foi sua experiência na Sprint#01 do programa de bolsa @node.js_mar22 e quais suas expectativas a partir de agora:
> Uma experiência totalmente nova! Muito empolgada com todo aprendizado até aqui! A começar da dinâmica diferente de tudo que já vi! Senti uma diferença muito grande, de forma positiva, muito produtiva! Vou aplicar tudo o que aprendi nessa primeira Sprint, corrigir alguns pontos que acho necessário melhorar! E dessa forma, pretendo ser melhor na próxima Sprint e aprender muito mais!
