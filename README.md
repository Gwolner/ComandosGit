# Comandos Git

Reposit�rio usado para praticar comandos git.

## 1 - Reposit�rio

### Criando um Reposit�rio

Todo repositorio Git armazena as informa�oes dentro de uma pasta oculta chamada "/.git". 
Para que os arquivos de uma pasta possam ser versionados pelo Git, � preciso iniciar o reposit�rio.
Para isso, execute o comando:

```
git init
```

## 2 - Branches

### Listando altera�oes

Esse comando lista todos os arquivos que foram modificados desde o seu �ltimo commit.

```
git status
```

### Listando Branches

Lista todos os branches presentes no reposit�rio local.

```
git branch
```

Lista todos os branches presentes no reposit�rio remoto.

```
git checkout minha-branch
```

### Excluindo branches

Excluir uma branch local com -d � mais segura, pois ela s� apaga a branch se voce j� tiver feito merge 
ou enviado as altera�oes para seu reposit�rio remoto, evitando perda de c�digo.

```
git branch -d nome-da-branch
```

Excluir uma branch local com -D � ignora o estado da sua branch, for�ando a sua remo�ao.

```
git branch -D nome-da-branch
```

### Subir branch local para reposit�rio

```
git push origin nome-da-branch
```

### Puxar branch do reposit�rio para o local

```
git checkout -track origin/nome-da-branch
```

## 3 - Commits

###  Hist�rico de Commits

visualizar o hist�rico de commits.

```
git log
```

### 





```

```

### 





```

```

### 





```

```

### 





```

```

### 





```

```

### 





```

```
















