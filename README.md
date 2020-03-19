# Comandos Git

Repositório usado para prática e registro de comandos Git.

O intúito deste repositório é servir de <b>consulta</b>, não como "passo-a-passo", ou seja, não existe uma sequencia a ser seguida. 

Se precisar de comandos para o repositorio local, basta consultar o tópico que trata disto. Precisa de comandos de branch? Vá para o tópico que trata delas. E assim por diante.

Este documento faz uso de imagens (emojis) para facilitar a compreensão do comando com o contexto que se é utilizado. Muitos dos repositórios existentes no Github usam apenas recurso textual, gerando certa dificuldade no leitor em se localizar na estrutura do Git.

Abaixo, um resumo deste documento: 

* [Estrutura Git](https://github.com/Gwolner/comandos-git#estrutura-git)
* [Repositório local](https://github.com/Gwolner/comandos-git#repositório-local-computer)
* [Container/Stage](https://github.com/Gwolner/comandos-git#containerstage-postbox)
* [Projeto](https://github.com/Gwolner/comandos-git#projeto-file_folder)
* [Commit](https://github.com/Gwolner/comandos-git#commits-pushpin)
* [Branch](https://github.com/Gwolner/comandos-git#branches-cactus)

## Estrutura Git

<b>:file_folder: Projeto --> :postbox: Container/Stage --> :computer: Repositório local --> :cloud: Repositório remoto</b>

## Repositório local :computer:

### :computer: Criando um Repositório

Todo repositorio Git armazena as informaçoes dentro de uma pasta oculta chamada "/.git". 
Para que os arquivos de uma pasta possam ser versionados pelo Git, é preciso iniciar o repositório.
Para isso, execute o comando:
```
git init
```

### :computer: Atualizar repositório remoto

Envia alterações do repositorio local para o repositório remoto.
```
git push
```

### :computer: Atualizar repositório local

Atualizar o repositório local com a versão mais recente do repositório remoto.
```
git pull
```

## Container/Stage :postbox:

### :postbox: Listando alteraçoes

Lista todos os arquivos e diretórios modificados/criados no projeto em relação ao último commit do container.
```
git status
```

### :postbox: Enviando alterações para o repositório local

Envia para o repositório local a ultima modificação realizada no container, além de permitir uma mensagem que explique essa modificação. 
```
git commit -m "mensagem"
```

## Projeto :file_folder:

### :file_folder: Adicionar alteraçõs do projeto ao container.

Arquivos específicos.
```
git add nome-arquivo.extensao
```

Todos os arquivos alterado ou criados.
```
git add .
```

## Commits :pushpin:

### :pushpin: Histórico 

Visualizar o histórico de commits.
```
git log
```

Histórico de commits resumido.
```
git log --oneline
```

### :pushpin: Visualização gráfica

Histórico de commits com gráfico.
```
git log --graph
```

Histórico de commits com gráfico.
```
git log --graph
```

## Branches :cactus:

### :cactus: Criando uma branch

```
git checkout -b minha-nova-branch
```

### :cactus: Listando branches

Lista branches presentes no repositório local.
```
git branch
```

Lista branches presentes no repositório remoto.
```
git branch -a
```

### :cactus: Alternando entre branches

```
git checkout minha-branch
```

### :cactus: Excluindo branches

Excluir uma branch local com -d só irá apagar a branch se voce já tiver feito merge 
ou enviado as alteraçoes para seu repositório remoto, evitando perda de código.
```
git branch -d nome-da-branch
```

Excluir uma branch local com -D é ignora o estado da sua branch, forçando a sua remoçao.
```
git branch -D nome-da-branch
```

### :cactus: Subir branch local para repositório

```
git push origin nome-da-branch
```

### :cactus: Puxar branch do repositório para o local

```
git checkout -track origin/nome-da-branch
```
