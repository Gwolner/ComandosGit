# Comandos Git

Repositório usado para praticar comandos git.

## 1 - Repositório

### Criando um Repositório

Todo repositorio Git armazena as informaçoes dentro de uma pasta oculta chamada "/.git". 
Para que os arquivos de uma pasta possam ser versionados pelo Git, é preciso iniciar o repositório.
Para isso, execute o comando:

```
git init
```

## 2 - Branches

### Listando alteraçoes

Esse comando lista todos os arquivos que foram modificados desde o seu último commit.

```
git status
```

### Listando Branches

Lista todos os branches presentes no repositório local.

```
git branch
```

Lista todos os branches presentes no repositório remoto.

```
git checkout minha-branch
```

### Excluindo branches

Excluir uma branch local com -d é mais segura, pois ela só apaga a branch se voce já tiver feito merge 
ou enviado as alteraçoes para seu repositório remoto, evitando perda de código.

```
git branch -d nome-da-branch
```

Excluir uma branch local com -D é ignora o estado da sua branch, forçando a sua remoçao.

```
git branch -D nome-da-branch
```

### Subir branch local para repositório

```
git push origin nome-da-branch
```

### Puxar branch do repositório para o local

```
git checkout -track origin/nome-da-branch
```

## 3 - Commits

###  Histórico de Commits

visualizar o histórico de commits.

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
















