# Diff

O comando diff pode ser usado para ver diferenças entre commits e estados da working tree

## Sem argumentos

Caso você rode o diff sem argumentos, ele vai mostrar a diferença entre alterações ainda não commitadas
em relação ao último commit. Caso o status esteja limpo, o comando não mostra nada

	git diff

## Entre dois commits

Podemos então ver a diferença entre dois commits da seguinte maneira:

	git diff <hash do mais antigo>..<hash do mais novo>

Isso vai mostrar as diferenças entre o commit mais antigo até o mais novo
