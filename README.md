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
