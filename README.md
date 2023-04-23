# Config-Git

[push]

	followTags = true
  
[alias]

	c = !git add --all && git commit -m
  
	s = !git status -status
  
	l = !git log --pretty=format:'%C(blue)%h%C(red)%d %C(white)%s - %C(cyan)%cn, %(green)%cr'
	amend = !git add --all && git commit --amend --no-edit
	count = !git shortlog -s --grep



## Descrição:

`git config --global core.editor code`

Este comando define o editor de texto padrão para o Git. O editor definido aqui é o "Visual Studio Code" (VS Code), pois o comando "code" é o atalho para abrir o VS Code. Caso prefira usar outro editor, substitua "code" pelo comando de abertura do seu editor.

`git config --global --edit`

 Este comando abre o arquivo de configuração do Git no seu editor padrão, permitindo a edição de várias configurações, como nome e endereço de email, opções de formatação de logs, opções de merge, entre outras.

`[push] followTags = true`

 Este é um bloco de configuração para o comando git push. A opção followTags é definida como true, o que significa que, ao fazer um git push, as tags (etiquetas) criadas localmente serão enviadas para o repositório remoto.

`[alias]`

Este bloco de configuração define alguns atalhos (aliases) para comandos Git. Cada alias é definido com uma letra, que será usada para chamar o comando posteriormente.

`c = !git add --all && git commit -m`

 Este alias define o comando "c" para executar uma sequência de dois comandos: "git add --all" (que adiciona todos os arquivos modificados ao stage) e "git commit -m" (que realiza o commit com a mensagem especificada). Para usar este alias, basta digitar "git c" no terminal e digitar a mensagem de commit.

`s = !git status -status`

Este alias define o comando "s" para executar o comando "git status" com a opção "-status", que exibe uma versão resumida do status do repositório.

`l = !git log --pretty=format:'%C(blue)%h%C(red)%d %C(white)%s - %C(cyan)%cn, %(green)%cr'`

Este alias define o comando "l" para executar o comando "git log" com uma opção de formatação personalizada. Essa opção de formatação define como o log deve ser exibido no terminal, incluindo as cores usadas para destacar informações importantes.

`amend = !git add --all && git commit --amend --no-edit`

Este alias define o comando "amend" para executar a sequência de comandos "git add --all" e "git commit --amend --no-edit". Isso permite que você adicione novas alterações ao commit anterior, sem precisar editar a mensagem de commit.

`count = !git shortlog -s --grep`

Este alias define o comando "count" para executar o comando "git shortlog" com a opção "-s --grep", que conta o número de commits que contém uma determinada palavra-chave (no lugar de grep). É útil para contabilizar contribuições de desenvolvedores em projetos open-source, por exemplo.


