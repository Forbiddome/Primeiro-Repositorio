$ git push origin main
git status
To https://github.com/USERNAMEX/Primeiro-Projeto.git
 ! [rejected]        main -> main (fetch first)
error: failed to push some refs to 'https://github.com/USERNAMEX/Primeiro-Repositorio.git'
hint: Updates were rejected because the remote contains work that you do
hint: not have locally. This is usually caused by another repository pushing
hint: to the same ref. You may want to first integrate the remote changes
hint: (e.g., 'git pull ...') before pushing again.
hint: See the 'Note about fast-forwards' in 'git push --help' for details.

Caso não conseguido dar o Push do commit por conta desse erro é porque houve uma modificação no
repositório remoto e enquanto você não tiver trocado o seu repositorio local pelo atual repositorio remoto 
aparecerá esse erro. O erro é devido a necessidade de sincronização das versões. Esse é o principal
propósito do Git - ser um gerenciador de versões múltiplas distribuídas(logo precisam estar sincronizadas)
e no caso de estarmos usando o GitHub o controle de versionamento é remoto.

# 
Para isso basta repetir os passos do arquivo PARTE 2 aqui nesse mesmo repositório
lembrando de apagar o seu repositório local por completo e usando o git clone "link"
novamente e ai sim usando o git commit -m "coloque a msg aqui" agora sim podendo modicar o remoto #
