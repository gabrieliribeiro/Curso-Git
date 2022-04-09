
### ╭━━━━━━━━ GIT E GITHUB ━━━━━━━━ 📚✏️ 

### ╰┈┈┈➤ O que é controle de versão ? 

* Uma técnica que ajuda a gerenciar o código-fonte de uma aplicação;
* Registrando todas as modificações de código, podendo também reverter as mesmas;
* Criar versões de um software em diferentes estágios, podendo alterar facilmente entre elas;
* Cada membro da equipe pode trabalhar em uma versão diferente;
* Há ferramentas para trabalhar o controle de versão: git e SVN.

### ╰┈┈┈➤ O que é Git ? 

* O sistema de controle de versão mais utilizado do mundo atualmente;
* O git é baseado em repositórios, que contêm todas as versões do código e também as cópias de cada desenvolvedor;
* Todas as operações do git são otimizadas para ter alto desempenho;
* Todos os objetivos do git são protegidos com criptografia para evitar alterações indevidas e maliciosas;
O git é um projeto de código aberto.

 ### ╰┈┈┈➤ Criando repositórios 
 * Para criar um repositório utilizamos o comando *git init*;
 * Desta maneira o git vai criar os arquivos necessários para inicializá-los;
 * Que estão na pasta oculta *.git*;
 * Após este comando o diretório atual será reconhecido pelo git como um projeto e reponderá aos seus demais comandos.

 ### ╰┈┈┈➤ Enviando repositórios para o GH 
  
 ##### ➔ COMANDOS FUNDAMENTAIS :
* *git init* ( para novos repositórios)
* *git status*
* *git add < file >* ( add . <seleciona todos os arquivos>)
* *git commit < files > (-a < todos >) -m ""*
* *git push*
* *git pull* (buscando att)
* *git clone* (clonar repositório) 
* *git rm* (deletar arquivos)
* *git log* (receber informações) (ctrl+q pra sair)
* *git mv* (renomear arquivos/mover para outra pasta)
  (para renomear: *git mv < file > < file att >* )
* *git checkout <file>* (retornado ao estado original)
* *.gitignore* (ignorar arquivos)
* *git reset* (geralmente usado com a flag --hard) origin/main

###  ╰┈┈┈➤ Branches
 
  #### ➔ O que é um branch?	
 * Branch é a forma que o git separa as versões dos projetos;
 * Quando um projeto é criado ele inicia na branch main;
 * Geralmente cada nova feature de um projeto fica em um branch separado;
 * Após a finalização das alterações os branchs são unidos para ter o código-fonte final.
 
###  ╰┈┈┈➤ Criando e vizualizando Branches
 * *git branch* (para vizualiizar)
 * *git branch < nome >* (para criar)
 
 ###  ╰┈┈┈➤ Deletando Branches
  * *-d ou --delete*
  * Não é comum deletar um branch, pois normalmente se guarda o histórico do trabalho;
  * Ele é geralmente usado quando o branch foi criado errado.
  
 ###  ╰┈┈┈➤ Mudando de Branch
  * Podemos mudar para outro branch utilzando o comando: *git checkout -b < nome >* 
  * Este comando também é utilizado para dispensar mudanças de um arquivo;
  * Alterando o branch podemos levar alterações que não foram commitadas junto, **tome cuidado!** .
 
 ###  ╰┈┈┈➤ Unindo Branchs
  * O código de dois branches distintos pode ser unido pelo comando: *git merge < nome >*
  * Esse seria mais um comando para a lista de mais utilizados;
  * Normalmente é por meio dele que recebemos as atualizações de outros devs.
 
 ###  ╰┈┈┈➤ Stash
  * Podemos salvar modificações atuais para prosseguir com uma outra abordagem de solução e não perder o código;
  * O comando para esta ação é o: *git stash*;
  * Após o comando o branch será resetado par sua versão de acordo com o repo.
 
 ###  ╰┈┈┈➤ Recuperando Stash
  * Podemos verificar as stashs criadas pelo comando: *git stash list*;
  * E também podemos recuperar com o comando: *git stash apply < nome >*;
  * Podemos ver as alterações delas com : *git stash show -p < nome >*;
  * Dessa maneira podemos continuar de onde paramos com os arquivos adicionados a stash.
 
  ###  ╰┈┈┈➤ Removendo Stash
   * Para limpar totalmente as stash de um branch podemos utilizar o comando: *git stash clear*;
   * Caso seja necessário deletar uma stash específica podemos utilizar: *stash drop < nome >*.
 
 ###  ╰┈┈┈➤ Utilizandos Tags
   * Podemos criar tags nos branchs por meio do comando : *git tag -a < nome > -m "< msg >"*;
   * A tag é diferente do stash, serve como um **checkpoint de um branch**;
   * É utilizada para demarcar estágios do desenvolvimento de algum recurso.
 
 (ﾉ◕ヮ◕)ﾉ*✲ﾟ*｡⋆





