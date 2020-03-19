# Comandos Git

Repositório usado para praticar comandos git com registro dos comandos já aprendidos.

* Estrutura
* Comandos iniciais - Master
  * 1 - Repositório remoto
  * 2 - Repositório local
  * 3 - Projeto
  * 4 - Container/Stage
* Comandos específicos - Branch & Commit
* Terminal Bash


## Estrutura

<b>Projeto :file_folder: --> Container/Stage :postbox: --> Repositório local :computer: --> Repositório remoto :cloud:</b>

<i><b>IMPORTANTE!</b></i>
Para que exista um container é preciso que primeiro exista um repositório local. Não há como criar o container e depois o repositório local. Sendo assim, será abordado primeiro os comandos do repositorio e, logo em seguida, os comandos do container.



## Comandos iniciais - Master

### 1 - Repositório remoto

#### :cloud: Baixar repositório remoto.

Pode-se baixar um repositório remoto para um PC desde que se conheça se endereço.
```
git clone endereço-repositorio
```

### 2 - Repositório local

#### :computer: Criando um Repositório

Todo repositorio Git armazena as informaçoes dentro de uma pasta oculta chamada "/.git". 
Para que os arquivos de uma pasta possam ser versionados pelo Git, é preciso iniciar o repositório.
Para isso, execute o comando:
```
git init
```

#### :computer: Atualizar repositório remoto

Envia alterações do repositorio local para o repositório remoto.
```
git push
```

#### :computer: Atualizar repositório local

Atualizar o repositório local com a versão mais recente do repositório remoto.
```
git pull
```

### 3 - Projeto

#### :file_folder: Adicionar alteraçõs do projeto ao container.

Arquivos específicos.
```
git add nome-arquivo.extensao
```

Todos os arquivos alterado ou criados.
```
git add .
```
Ou 
```
git add *
```
#### :file_folder: Criar arquivo
```
touche nome-arquivo.extensao
```

### 4 - Container/Stage

#### :postbox: Listando alteraçoes

Lista todos os arquivos e diretórios modificados/criados no projeto em relação ao último commit do container.
```
git status
```

#### :postbox: Enviando alterações para o repositório local

Envia para o repositório local a ultima modificação realizada no container, além de permitir uma mensagem que explique essa modificação. 
```
git commit -m "mensagem"
```

## Comandos específicos - Branch & Commit

### 6 - Commits

Visualizar o histórico de commits.
```
git log
```

Histórico de commits resumido.
```
git log --oneline
```

Histórico de commits com gráfico.
```
git log --graph
```

Histórico de commits com gráfico.
```
git log --graph
```

### 7 - Branches

#### :cactus: Criando uma branch
```
git checkout -b minha-nova-branch
```

#### :cactus: Listando branches

Lista todos os branches presentes no repositório local.
```
git branch
```

Lista todos os branches presentes no repositório remoto.
```
git branch -a
```

#### :cactus: Alternando entre branches
```
git checkout minha-branch
```

#### :cactus: Excluindo branches

Excluir uma branch local com -d só irá apagar a branch se voce já tiver feito merge 
ou enviado as alteraçoes para seu repositório remoto, evitando perda de código.
```
git branch -d nome-da-branch
```

Excluir uma branch local com -D é ignora o estado da sua branch, forçando a sua remoçao.
```
git branch -D nome-da-branch
```

#### :cactus: Subir branch local para repositório
```
git push origin nome-da-branch
```

#### :cactus: Puxar branch do repositório para o local
```
git checkout -track origin/nome-da-branch
```



## Terminal Bash

:desktop_computer: Exibir conteúdo de um diretório.
```
ls
```

:desktop_computer: Limpar a tela.
```
clear
```

