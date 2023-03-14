# Repos Remotos

Podemos criar repositório que são repositórios comum e repositórios "bare".
Repositórios bare são repos que não guardam cópias dos arquivos, apenas suas alterações (não tem a working tree)
com isso podemos usar este repositório bare feito a mão como um repositório remoto para outro repo comum

O comando é o seguinte:

	git init --bare

## Repos Remotos para Repos comuns

Ao ter um repositório remote, onde quer que seja, podemos listar os repos remotos conhecidos:
	
	git remote

Caso não haja repos remotos ainda, podemos adicioanar:

	git remote add <nome: a convencao e origin> <caminho local ou remoto>

Para checkar tanto o nome quanto o endereço dos remotes conhecidos, usamos o seguinte: 
	
	git remote -v

Caso queiramos mudar o nome de um repo remoto, podemos usar o seguinte

	git remote rename <nome velho> <nome novo>

## Fazendo um Push

Para fazer um push, o padrão de como ele realmente funciona é o seguinte

	git push <nome do remoto> <branch desejada>


Caso queiramos usar apenas `git push`, podemos fazer o seguinte comando no primeiro push:

	git push -u <remoto> <branch>

Após isso ser configurado, apenas `git push` será suficiente
