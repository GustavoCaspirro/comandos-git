# Comandos Git

## CONFIGURE A FERRAMENTA
Configure informações de usuário para todos os repositórios locais.

- Configura o nome que você quer ligado as suas transações de
commit
```sh
$ git config --global user.name "[nome]"
```
- Configura o email que você quer ligado as suas transações de commit
```sh
$ git config --global user.email "[endereco-de-email]"
```

## CRIE REPOSITÓRIOS
Inicie um novo repositório ou obtenha de uma URL existente

- Cria um novo repositório local com um nome específico
```sh
$ git init [nome-do-projeto]
```
- Baixa um projeto e seu histórico de versão inteiro
```sh
$ git clone [url]
```

## FAÇA MUDANÇAS
Revise edições e crie uma transação de commit

- Lista todos os arquivos novos ou modificados para serem commitados
```sh
$ git status
```

- Faz o snapshot de um arquivo na preparação para versionamento
```sh
$ git add [arquivo]
```

- Deseleciona o arquivo, mas preserva seu conteúdo
```sh
$ git reset [arquivo]
```
- Mostra diferenças no arquivo que não foram realizadas
```sh
$ git diff
```
- Mostra a diferença entre arquivos selecionados e a suas últimas versões
```sh
$ git diff --staged
```
- Grava o snapshot permanentemente do arquivo no histórico de versão
```sh
$ git commit -m "[mensagem descritiva]"
```

## MUDANÇAS EM GRUPO
Nomeie uma série de commits e combine os esforços completos

- Lista todos os branches locais no repositório atual
```sh
$ git branch
```

- Lista todos os branches
```sh
$ git branch -a
```

- Cria um novo branch
```sh
$ git branch [nome-do-branch]
```

- Muda para o branch específico e atualiza o diretório de trabalho
```sh
$ git checkout [nome-do-branch]
```

- Cria e Muda para o branch específico e atualiza o diretório de trabalho
```sh
$ git checkout -b [nome-do-branch]
```

- Limpa e e atualiza os arquivos que não foram adicionados
```sh
$ git checkout .
```

- Combina o histórico do branch específico com o branch atual
```sh
$ git merge [branch]
```

- Exclui o branch específico
```sh
$ git branch -D [nome-do-branch]
```

## REFATORE NOMES DOS ARQUIVOS
Mude e remova os arquivos versionados

- Remove o arquivo do controle de versão mas preserva o arquivo localmente
```sh
$ git rm --cached [arquivo]
```

- Remove o arquivo do diretório de trabalho e o seleciona para remoção
```sh
$ git rm [arquivo]
```

- Muda o nome do arquivo e o seleciona para o commit
```sh
$ git mv [arquivo-original] [arquivo-renomeado]
```

## REVISE HISTÓRICO
Navegue e inspecione a evolução dos arquivos do projeto

- Lista o histórico de versões para o branch atual
```sh
$ git log
```

- Lista o histórico de versões para um arquivo, incluindo mudanças de nome
```sh
$ git log --follow [arquivo]
```

- Mostra a diferença de conteúdo entre dois branches
```sh
$ git diff [primerio-branch]...[segundo-branch]
```

- Retorna mudanças de metadata e conteúdo para o commit especificado
```sh
$ git show [commit]
```

## DESFAÇA COMMITS
Apague enganos e crie um histórico substituto

- Desfaz todos os commits depois de `[commit]`, preservando mudanças locais
```sh
$ git reset [commit]
```

- Descarta todo histórico e mudanças para o commit especificado
```sh
$ git reset --hard [commit]
```

## SINCRONIZE MUDANÇAS
Registre um marcador de repositório e troque o histórico de versão

- Limpa arquivos de backup do merge
```sh
$ git clean [marcador]
```

- Baixe todo o histórico de um marcador de repositório
```sh
$ git fetch [marcador]
```

- Combina o marcador do branch no branch local
```sh
$ git merge [marcador]/[branch]
```

- Envia todos os commits do branch local para o GitHub
```sh
$ git push [alias] [branch]
```

- Baixa o histórico e incorpora as mudanças
```sh
$ git pull
```
