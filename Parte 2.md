# Inicialização simplificada do uso do Git/GitHub #
##

1.  Baixe e instale o Git, em seguida abra o GitBash
2.  Crie um Repositório no GitHub com um arquivo para eventual teste
3.  Copie o link HTTPS do repositório no site GitHub cliquando em CODE(em fundo verde)
4.  Na Janela do GitBash escreva: "git clone (acompanhado do link que HTTPS)" para clonar o Repositório remoto no seu PC
5.  Agora entre na pasta do repositorio digitando cd "nome do repositório"
6.  Novamente no GitBash digite git status para verificar se tem algo novo no repositorio local a ser entregado(commitado) ao remoto
##

### Caso não modifique nada no repositório baixado aparecerá a mensagem ###

$ git status
On branch main
Your branch is up to date with 'origin/main'.

nothing to commit, working tree clean

### Caso modifique algo no repositório baixado aparecerá a mensagem de exemplo ###

$ git status
On branch main
Your branch is up to date with 'origin/main'.

Untracked files:
  (use "git add <file>..." to include in what will be committed)
        Segunda pasta/

nothing added to commit but untracked files present (use "git add" to track)
  
## 7.  Após isso escreve-se git add . (com auxilio da flag . ou -A) para adicionar tudo que seja novo ao seu repositório local ##
caso digite git status aparecerá
  
Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   Segunda pasta/texto2.txt


## 8.  Agora para "Empacotar" o repositorio local para reenvia-lo para o remoto use git commit ##
Caso seja sua Primeira vez com o Git aparecerá o seguinte aviso de erro

$ git commit
Author identity unknown

*** Please tell me who you are.

Run

  git config --global user.email "you@example.com"
  git config --global user.name "Your Name"

to set your account's default identity.
Omit --global to set the identity only in this repository.

fatal: unable to auto-detect email address (got 'USERNAMEX@PC-DO-USERNAMEX.(none)')

### Como pedido na descrição do erro, basta adicionar um name e um email ao git 
config usando as instruções dadas além disso aparecerá um aviso pedindo que você 
escreva uma mensagem para o commit
  
  Lembrando que esse email e name se tratam de créditos de autoria da modificação
  e não as credenciais para poder modificar o repositorio é falado em Parte 4###
  

Please enter the commit message for your changes. Lines starting
with '#' will be ignored, and an empty message aborts the commit.
On branch main
Your branch is up to date with 'origin/main'.
Changes to be committed:
       new file:   Parte-4.txt

### Para sair dessa tela aperte "ctrl + c" depois disso digite ":qa" aperte enter e agora digite
[git commit -m "uma mensagem de sua autoria que referencia a esse commit"] (usando aspas mesmo) ###

  $ git commit -m "adicionando segunda pasta"
[main e3824c5] adicionando segunda pasta
 1 file changed, 1 insertion(+)
 create mode 100644 Segunda pasta/texto2.txt
  
## 9. veja por uma ultima vez o status do seu repositorio local com git status aparecerá ##
$ git status
On branch main
Your branch is ahead of 'origin/main' by 1 commit.
  (use "git push" to publish your local commits)

nothing to commit, working tree clean

### Agora escreva no GitBash git push origin main ###
  
## 10 Fim! 
Agora dê uma olhada no seu GitHub e Pronto! ##

