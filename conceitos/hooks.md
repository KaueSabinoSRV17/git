# Hooks

Podemos adicionar scripts Bash (ou qualquer outra linguagem, como Python) que são disparados
após algumas ações do git

Os Scripts devem estar na pasta `hooks/`, dentro da pasta `.git`.

Garanta que pelo menos o usuário dono do arquivo (você mesmo, que criou ele) possa executar-lo
com o seguinte comando: 

	chmod u+x <arquivo do hook>

O arquivo deve seguir o seguinte padrão: 

- Não deve ter extensão
- Deve ser executável (garanta isso com o comando acima)
- Seu nome deve ser igual a um dos arquivos .sample que está na pasta dos Hooks
