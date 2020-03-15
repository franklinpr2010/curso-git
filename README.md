
# Curso de Git. 

### Branches

Criações de novas branches para desenvolver novas interações no projeto sem afetar o branch principal, isso garante que as pessoas não obtenham erros ao fazer novos commits, isso não afetará a linha principal do projeto. É como se fosse uma linha paralela.

Quando quer restaurar na branch master terá que fazer um merge para introduzir o conteúdo para a branch principal, quando isso acontece é porque estamos fazendo um merge Fast-forward, isso significa que pegará os commits e anexará a branch master para fazer novas alterações sem precisar criar novos commits.

Crie um projeto no VSC.

> git init

Crie um arquivo : Arquivo1.txt

> git add . (Adiciona na stage)

> git commit -m "primeiro"

Crie agora uma nova Branch

>  git branch nova-branch

Averigue se deu certo

> git branch

Pule para uma nova branch (Todas as alterações estarão na nova branch)

> git checkout nova-branch



















