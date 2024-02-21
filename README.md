# Aula de POO 

Lista da equipe

- Caio Henrique Nunes Viana
- Matheus Marcelino da Silva
- Joana da Silva
- Jamilly da Silva Pinheiro

## COMANDOS

### INIT

- É o primeiro programa executado pelo kernel durante a inicialização. Por padrão, o processo init é identificado no sistema com o número 1, ou seja, o PID do init é 1 (a identificação dos processos em execução pode ser visto no diretório /proc). 



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

### PUSH
Enviar arquivos/diretórios para o repositório remoto:

O primeiro push de um repositório deve conter o nome do repositório remoto e o branch:
```java
git push -u origin master
``````
Os demais pushes não precisam dessa informação:
```java
git push
``````

