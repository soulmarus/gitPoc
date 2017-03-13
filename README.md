# gitPoc
POC de utilização de GIT

1) Para Clonar um repositorio 

git clone usuário@servidor:/caminho/para/o/repositório
		  macario@https://github.com/soulmarus/gitPoc.git

2) Após modificar um arquivo ou cria-ló proponha a mudança (adicioná-las ao Index) executando o comando:

	git add <arquivo>
	git add *

	Obs.: Este é o primeiro passo no fluxo de trabalho básico do git
	
3) Para realmente confirmar as mudanças feitas é necessario realizar executar o comando commit:

	git commit -m "comentários das alterações"