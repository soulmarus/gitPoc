# gitPoc
POC de utilização de GIT

Obtenha um repositório

1) Para Clonar um repositorio 

git clone usuário@servidor:/caminho/para/o/repositório
		  macario@https://github.com/soulmarus/gitPoc.git

Adicionar & Confirmar

1) Após modificar um arquivo ou cria-ló proponha a mudança (adicioná-las ao Index) executando o comando:

	git add <arquivo>
	git add *

	Obs.: Este é o primeiro passo no fluxo de trabalho básico do git
	
2) Para realmente confirmar as mudanças feitas é necessario realizar executar o comando commit:

	git commit -m "comentários das alterações"
	
3) Para enviar as alterações, suas alterações agora estão no HEAD da sua cópia de trabalho local. 
   Para enviar estas alterações ao seu repositório remoto, execute :

	git push origin master
	
	Obs.: Altere master para qualquer ramo (branch) desejado, enviando suas alterações para ele. 
	
Ramificando

1) Para criar um novo branch chamado "funcionalidade_x" e seleciona-ló use o comando abaixo:

	git checkout -b funcionalidade_x
	
2) Para listar todos os branch locais utilize o comando:

	git branch

3) Para navegar entre branches utilizando o comando:

	git checkout <branch>
	
4) Para remover uma branch utilize o comando abaixo:

	git branch -d funcionalidade_x
	
	Obs.: Um branch não está disponível a outros a menos que você envie o branch para seu repositório remoto.
	
	git push origin <funcionalidade_x>

Atualizar & Mesclar

1) Para atualizar seu repositório local com a mais nova versão, execute o comando abaixo na sua pasta de trabalho para obter e fazer merge (mesclar) alterações remotas.:
	
	git pull	
	
2) Para fazer merge de um outro branch ao seu branch ativo (ex. master), use:

	git merge <branch>
	
3) Em ambos os casos o git tenta fazer o merge das alterações automaticamente. Infelizmente, isto nem sempre é possível e resulta em conflitos. Você é responsável por fazer o merge estes conflitos manualmente editando os arquivos exibidos pelo git. Depois de alterar, você precisa marcá-los como merged com:

	git add <arquivo>
	
Fonte: http://rogerdudler.github.io/git-guide/index.pt_BR.html