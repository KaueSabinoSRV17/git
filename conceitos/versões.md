# Versões

Pelo git podemos manipular versões de diversas formas...

## Descartar alterações não commitadas

Podemos usar o:

	git checkout <caminho de arquivos com mudanças a ser descartadas>

**Lembrando que caminhos no git são recursivos, então caso você queira descartar de uma pasta inteira ou todo o projeto, passe o caminho da pasta**

## Descartar alterações no stage

Para tirar do stage

	git reset HEAD <arquivo a sair do stage>

## Descartar alterações já commitadas

Para desfazer um commit feito, é uma boa prática usar o comando `revert` que vai desfazer um commit através de sua hash
e automaticamente atribuir essa ação a um novo commit

	git revert <hash do commit a ser desfeito>

## Stash

Para poder salvar modifiações, sem commita-las, podemos usar o `stash`. 
Ele é útil para um momento onde fizemos muito trabalho, que ainda não deve ser commitado, e precisamos fazer outra coisa, 
na mesma branch. 


### Comandos

Para salvar modificações em um stash

	git stash

Para listar todos os stashes

	git stash list

Para mostrar o que muda em cada stash

	git stash show -p <índice do stash, visto no list>

Para aplicar as modificações de um stash (o stash ainda vai existir depois disso)
	
	git stash apply <índice do stash>

Para apagar um stash, idealmente após o apply

	git stash drop <índice do stash>

Para aplicar e apagar ao mesmo tempo

	git stash pop <índice do stash>
