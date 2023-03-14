# Branches

Quando queremos separar o projeto em linhas diferentes de desenvolvimento, podemos usar branches
Branches nada mais são do que um ramo com alterações isoladas da master. Devemos separar o código
de features ainda não concluida da main, para que, por exemplo, quando for necessário a correção de um bug,
não seja necessária a integração de código ainda não finalizado para dentro da main

## Comandos

Para listar branches...

	git branch

Para criar nova

	git branch <nova branch>

Para mudar de branch

	git checkout <branch diferente da sua atual>

Bônus: cria branch e já entra dentro dela

	git checkout -b <nova branch>

## Unindo trabalho

Assim que garantimos que todo o código da branch em que estamos trabalhando está validado, podemos
juntar o que adicionamos nela com a branch main. Para isso, temos 2 comandos diferentes

Vale lembrar que os comandos não são de 2, parâmetros. São apenas um, no caso a branch onde
estão os commits a serem adicionados. A branch que vai receber os commits é sempre a sua branch atual,
então não se esqueça de fazer um checkout para a branch que será atualizada

### Merge

O Merge vai adicionar os commits da branch desejada na sua branch atual, e vai automáticamente
fazer um commit de merge.

#### Comando

O comando é:

	git merge <branch com alterações>

### Rebase

O Rebase nada mais é do que adicionar os commits da branch desejada na branch atual, mas sem
adicionar um commit de merge. No processo, alterações da branch atual estarão na frente das alterações
recebidas por outra branch, mas tudo estará junto

#### Comando

O comando é:

	git rebase <branch com alterações>
