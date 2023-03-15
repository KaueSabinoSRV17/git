# Cherry Pick

Podemos usar um cherry pick para trazer alterações de um commmit específico de outra branch.
No caso, apenas esse commit específico.

Isso pode ser útil quando voltamos para a `main` para realizar uma correção de bug, 
mas precisamos de uma alteração específica de um commit. Essa alteração pode estar em qualquer lugar
da linha do tempo desta outra branch

## Comando

o comando fica assim: 

**OBS: FAÇA CHECKOUT PARA A MASTER. O CHERRY-PICK TRÁS SEMPRE O COMMIT DE OUTRA BRANCH PARA A SUA ATUAL, MAS EM NENHUM MOMENTO ESPECIFICAMOS AS BRANCHES**

	git cherry-pick <hash do commit com a alteração desejada>
