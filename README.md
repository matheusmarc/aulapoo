# Aula de POO 

Lista da equipe

- Caio Henrique Nunes Viana
- Matheus Marcelino da Silva
- Joana da Silva
- Jamilly da Silva Pinheiro

## COMANDOS

### INIT

- O comando git init cria um novo repositório do Git. Ele pode ser usado para converter um projeto existente e não versionado em um repositório do Git ou inicializar um novo repositório vazio.



### git commit
Serve para comitar um arquivo/diretório

- Comitar um arquivo: ``` "git commit meu_arquivo.txt" ```

- Comitar vários arquivos: ``` "git commit meu_arquivo.txt meu_outro_arquivo.txt"```
- Comitar informando mensagem: ```"git commit meuarquivo.txt -m "minha mensagem de commit" ```
=======
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

