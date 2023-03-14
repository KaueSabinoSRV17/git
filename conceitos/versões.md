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
