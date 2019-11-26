# Comandos Git

## CONFIGURE A FERRAMENTA
Configure informações de usuário para todos os repositórios locais.

- Configura o nome que você quer ligado as suas transações de
commit
```sh
git config --global user.name "[nome]"
```
- Configura o email que você quer ligado as suas transações de commit
```sh
git config --global user.email "[endereco-de-email]"
```
- Configura o email que você quer ligado as suas transações de commit
```sh
git config --global color.ui auto
````

## CRIE REPOSITÓRIOS
Inicie um novo repositório ou obtenha de uma URL existente

- Cria um novo repositório local com um nome específico
```sh
git init [nome-do-projeto]
```
- Baixa um projeto e seu histórico de versão inteiro
```sh
git clone [url]
```
## FAÇA MUDANÇAS
Revise edições e crie uma transação de commit

- Lista todos os arquivos novos ou modificados para serem commitados
```sh
git status
```

- Faz o snapshot de um arquivo na preparação para versionamento
```sh
git add [arquivo]
```

- Deseleciona o arquivo, mas preserva seu conteúdo
```sh
git reset [arquivo]
```
- Mostra diferenças no arquivo que não foram realizadas
```sh
git diff
```
- Mostra a diferença entre arquivos selecionados e a suas últimas versões
```sh
git diff --staged
```
- Grava o snapshot permanentemente do arquivo no histórico de versão
```sh
git commit -m "[mensagem descritiva]"
```
