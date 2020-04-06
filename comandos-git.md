COMANDOS GIT

`git add .` - adiciona todas alterações<br>
`git add file.txt` - adiciona file.txt<br>
`git status` - vê estado dos commits<br>
`git status -s` - status resumido<br>
`git status --short` - status resumido<br>
`git commit -a` - commit direto, sem passar por stagging<br>
`git commit -m "Mensagem"` - commit passando pelo stagging com mensagem de alteração<br>
`git commit -amend` - adiciona alterações no commit anterior<br>
`git push origin master` - envia as alterações para o repositório na branch master<br>
`git push` - ||<br>
`git pull origin` - baixa commits do repositório remoto<br>
`git pull` - ||<br>
`git fetch origin` - atualiza as referências com um repositório remoto (busca branches etc)<br>
`git fetch` - ||<br>
`git rm <nome_do_arquivo>` - remove determinado arquivo do repositório local<br>
`git branch <nome_da_branch>` - cria nova branch com o nome desejado<br>
`git branch` - lista as branches disponíveis no repositório local<br>
`git checkout <nome_da_branch>` - navega para aquela branch<br>
`git checkout -b <nome_da_branch>` - cria nova branch e já faz checkout nela<br>
`git push --set-upstream origin new-branch` - faz push da nova branch e suas alterações<br>
`git push -u origin <nome_da_branch>` - faz push da branch (nova ou não) e suas alterações<br>
`git checkout -` - o git checkout - te leva a branch que você estava trabalhando antes de trocar de branch<br>
`git branch -d <nome_da_branch>` - remove branch do repositorio local<br>
`git push --delete origin <nome_da_branch>` - remove do repositório online a branch desejada<br>
`git merge <nome_da_branch>` - faz merge com a branch desejada<br>
`git merge <nome_da_branch> -no-ff` - faz merge com a branch deseja no modo 3-way<br>
`git pull --rebase` - força rebase ao fazer pull<br>
`git rebase <nome_da_branch>` - reaplica todos os commits na branch desejada<br>
`git rebase master -i` - mostra lista de commits e posso alterar ela para mudar o histórico e tudo, muito foda<br>
`git log` - mostra lista de commits<br>
`git log --oneline` - mostra historico de commits em uma linha por commit<br>
`git log --abbrev-commit` - ||<br>
`git log --color` - mostra historico de commits e tenta colorir o output<br>
`git log --graph` - mostra historico em um grafico das branchs em modo texto<br>
`git log --pretty` - mostra historico e permite que sejam utilizados place holders para as informações dos commits<br>
`git tag <versao>` - cria uma tag com a versao desejada<br>
`git checkout <versao>` - "travo" para usar aquele commit em específico<br>
`git push origin --tags` - além do push normal eu preciso fazer push das tags também, para acrescentar uma tag no que foi commitado<br>
`git checkout --ours <arquivo_conflito>` - adiciona conteúdo sem modificação que conflitou<br>
`git checkout --theirs` <arquivo_conflito> - adiciona conteúdo em conflito na branch atual que estou<br>
`git merge -abort` - cancela um merge que eu havia feito<br>
`git reset --mixed` - altera o staging e o repositório, mantém o working dir intacto. É o padrão e é útil nos casos que queremos desfazer partes das alterações e criar um novo commit em seguida<br>
`git reset --soft` - similar ao mixed, mas mantém o staging como está<br>
`git reset --hard` - desfaz tudo a partir de um commit específico<br>
`git revert` - não modifica histórico de commits, mas cria um novo commit com o inverso do commit desejado, ou seja, o resultado final é o commit anterior<br>
`git reset HEAD~1 --hard` - descarta e elimina as alterações do último commit<br>
`git checkout HEAD~2` - move o HEAD para dois commits anteriores<br>
`git revert <hash>` - reverte as alterações de um commit específico e cria um novo commit<br>
`git reset HEAD~2 <arquivo>` - restaura para o staging as alterações do arquivo desejado em dois commits atrás<br>
`git checkout -- <arquivo>` - recupera diretamente no working dir o arquivo desejado<br>
`git add --patch` - vejo linha por linha da alteração e consigo selecionar o que quero adicionar ao commit<br>
`git clone <repo> --depth` - quero o clone a partir de X commits<br>
