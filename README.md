
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
 
 ###  ╰┈┈┈➤ Verificando e atualizando Tags
   * Podemos verificar uma tag com o comando: *git show < nome >*;
   * Podemos trocar de tags com o comando: *git checkout < nome >*;
   * Desta maneira podemos retroceder ou avançar em checkpoints de um branch.
 
  ###  ╰┈┈┈➤ Enviando e compartilhando Tags
   * As tags podem ser enviadas para o repositório de código, sendo compartilhada entre os devs;
   * O comando é: *git push origin < nome >*;
   * Ou se quiser enviar mais tags: *git push origin --tags*.
 
 ###  ╰┈┈┈➤ Encontrando branchs
   * Branchs novos são criados a todo tempo e o seu git pode não estar mapeando eles;
   * Com o comando: *git fetch*, você é atualizado de todos os branchs e tags que ainda não estão reconhecidos por você;
   * Este comando é útil para utilizar o branch de algum outro dev do time, por exemplo.
   
 ###  ╰┈┈┈➤ Recebendo alterações
   * O comando: *git pull*, serve para recebermos atualizações do repositório remoto;
   * Cada branch pode ser atualizado com o *git pull*;
   * Utilizamos para atualizar a master do repo como também quando trabalhamos em conjunto e queremos receber as atualizações de um dev.
 
  ###  ╰┈┈┈➤ Enviando alterações
   * O comando: *git push*, faz o inverso do pull, ele envia as alterações para o repo remoto;
   * Serve também para **enviar as atualizações de um branch específico** para um outro dev;
   * Ou quando terminamos uma tarefa e precisamos enviar para o repo.
 
  ###  ╰┈┈┈➤ Utilizando o remote
   * Com o *git remote* podemos fazer algumas ações como: adicionar um repo para trackear ou remover;
   * Quando criamos um repo remoto, adicionamos ele ao git com *git remote add origin < link >*.
 
  ###  ╰┈┈┈➤ Trabalhando com submódulos
   * Submódulo é  a maneira que temos de possuir dois ou mais projetos em um só repositório;
   * Podemos adicionar uma depedência ao nosso projeto atual, porém mantendo suas estruturas separadas;
   * Para adicionar o submódulo utilizamos o comando: *git submodule add < repo >*;
   * Para verificar os submódulos o comando é : *git submodule*.
 
 ###  ╰┈┈┈➤ Atualizando submódulo
   * Para atualizar um submódulo primeiro devemos **comitar as mudanças**;
   * E para enviar para o repo do submódulo utilizamos: *git push --recurse-submodules=on-demand*;
   * Este fluxo fará a atualização apenas no submódulo.
 
 ###  ╰┈┈┈➤ Exibindo Inf
   * O comando: *git show*, nos dá diversas informações úteis;
   * Ele nos dá informações do branch atual e também de seus **commits**;
   * As **modificações de arquivos** entre cada commit também são exibidas;
   * Podemos exibir as informações de tags também com: *git show < tag >.
 
 ###  ╰┈┈┈➤ Exibindo Diferenças
   * O comando: *git diff* serve para exibir as diferenças de um branch;
   * Quando utilizado as diferenças do branch atual com o remoto serão exibidas no terminal;
   * Podemos também verificar a diferença entre arquivos com o comando: *git diff < arquivo > < arquivo_b >*.
 
 ###  ╰┈┈┈➤ Log Resumido
   * O comando: *git shortlog* nos dá um log resumido do projeto;
   * Cada commit será unido por **nome do autor**;
   * Podemos então saber quais commits foram enviados ao projeto e por quem;
   * Esse comando não tem nada haver com o branch e sim com o repositório.
 
 (ﾉ◕ヮ◕)ﾉ*✲ﾟ*｡⋆





