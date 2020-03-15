
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

Voltar para antiga branch

> git checkout master

Crie um novo arquivo chamado arquivo2.txt

> git add .

> git commit -m "commit 2"  

Agora vamos dar o merge com a branch master, na branch master:

Crie um novo arquivo na nova-branch

> Arquivo3.txt

> git add .

> git commit -m "commit 3"  

Vá para master

> git checkout master

Dê um merge dentro da branch master

> git merge nova-branch


## Graph - para averiguar a branch em forma de gráfico.

> git log --graph

Excluir um branch

> git branch -d nova-branch

### Outro exercicio

Crie uma branch chamada branch2, pode fazer direto dando o comando '-b'

> git checkout -b branch2

> git commit -am "merge final"


## Desfazendo operações e reset

Se quiser resetar as alterações antes de colocar na stage.

Crie um arquivo chamado palavra.txt

> git ckeckout palavra.txt

Remover algo que já esta na stage usa o comando reset.

> git reset head palavra.txt

Remover algo quando já foi comitado. Esse '^' é para ir para o anterior.

>git reset head^

Averigue se está no commit anterior

> git status

Para não precisar mais rastrear as alterações feitas nesse arquivo.

> git rm --cached palavra.txt

Para eliminar commits feitos previamente

> git reset --hard 9f2d0ea853a6139d4824878cc4356d4da16af3bf (hash do commit que se quer)






































