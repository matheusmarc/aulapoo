# Aula de POO 

Lista da equipe

- Caio Henrique Nunes Viana
- Matheus Marcelino da Silva
- Joana da Silva
- Jamilly da Silva Pinheiro

## COMANDOS

### INIT

- O comando git init cria um novo repositório do Git. Ele pode ser usado para converter um projeto existente e não versionado em um repositório do Git ou inicializar um novo repositório vazio.
  ```java
  git init
  ```
  ```java
  git init <diretório>
  ```

### STATUS

- O comando git status exibe as condições do diretório de trabalho e da área de staging. Ele permite que você veja quais alterações foram despreparadas, quais não foram e quais arquivos não estão sendo monitorados pelo Git.

```java
git status [<opções>…​] [--] [<pathspec>…​]
``````

### git commit
Serve para comitar um arquivo/diretório

- Comitar um arquivo: ``` "git commit meu_arquivo.txt" ```

- Comitar vários arquivos: ``` "git commit meu_arquivo.txt meu_outro_arquivo.txt"```
- Comitar informando mensagem: ```"git commit meuarquivo.txt -m "minha mensagem de commit" ```
<<<<<<< HEAD
=======
### ADD
- O comando git add não adicionará arquivos ignorados por padrão. Se algum arquivo ignorado for especificado explicitamente na linha de comando, git add falhará com uma lista de arquivos ignorados. Arquivos ignorados alcançados pela recursão de diretório ou globbing de nome de arquivo executado pelo Git (cite seus globs antes do shell) serão ignorados silenciosamente. O comando git add pode ser usado para adicionar arquivos ignorados com a opção -f (forçar).
  ```java
  git add
  ```


### log 

Exibir histórico:
```java
git log
``````
Exibir histórico com diff das duas últimas alterações:

```java
git log -p -2
``````
Exibir resumo do histórico (hash completa, autor, data, comentário e qtde de alterações (+/-)):

```java
git log --stat
``````

Exibir informações resumidas em uma linha (hash completa e comentário):

```java
git log --pretty=oneline
``````

Exibir histórico com formatação específica (hash abreviada, autor, data e comentário):

```java
git log --pretty=format:"%h - %an, %ar : %s"
``````
%h: Abreviação do hash;

%an: Nome do autor;

%ar: Data;

%s: Comentário.


O primeiro push de um repositório deve conter o nome do repositório remoto e o branch:
```java
git push -u origin master
```
Os demais pushes não precisam dessa informação:
```java
git push
```
### RESTORE

Restaure caminhos especificados na árvore de trabalho com algum conteúdo de uma fonte de restauração. Se um caminho for rastreado, mas não existir na origem de restauração, ele será removido para corresponder à origem.

O comando também pode ser usado para restaurar o conteúdo do índice com --staged ou restaurar a árvore de trabalho e o índice com --staged --worktree.

Por padrão, se --staged for fornecido, o conteúdo será restaurado do HEAD, caso contrário, do índice. Use --source para restaurar de um commit diferente.

Consulte "Redefinir, restaurar e reverter" no git[1] para ver as diferenças entre os três comandos.

ESTE COMANDO É EXPERIMENTAL. O COMPORTAMENTO PODE MUDAR.
```java
git restore 
```

### pull

```bash
git pull
```
- Usado para receber possíveis modificações feitas do servidor do Github