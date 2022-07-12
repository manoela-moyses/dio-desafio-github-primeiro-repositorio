# Desafio de Projeto sobre Git/GitHub da DIO :woman_technologist:

Olá! Bem vindo ao meu Desafio de Projeto :wave:



### Passo 1

Criar um repositório novo dentro da pasta _workspace_ no diretório (C:)

Abrir o Bash do Git direto no repositório

**_Comandos Git:_**

* **ls** (mostra todas as pastas contidas dentro do C:)

* **cd workspace/** (entra na pasta)

  _Obs.: **cd ..** (volta um nível)_

* **mkdir dio-desafio-github-primeiro-repositorio** (cria outra pasta dentro da pasta workspace)

* **cd dio-desafio-github-primeiro-repositorio/** (entra na pasta criada)

* **git init** (inicia o Git dentro dessa pasta)

* **ls -a** (essa flag -a mostra os arquivos ocultos)

  

### Passo 2

Se é a primeira vez que você está usando o Git, ele vai pedir algumas configurações iniciais

Ele vai pedir um _username_ (apelido) e um e-mail

_Obs.: seria interessante que o seu username e o seu e-mail fossem idênticos aos da plataforma on-line do GitHub_

**_Comandos Git:_**

* **git config --global user.email "seu e-mail aqui"**

* **git config --global user.name "seu nome aqui"**

  

### Passo 3

Criar um arquivo **Anotações.txt** dentro da pasta **dio-desafio-github-primeiro-repositorio**

**_Comandos Git:_**

* **echo > Anotações.txt**



### Passo 4

Commitar estes arquivos

_Obs.: tudo o que está no seu repositório local tem que estar commitado; caso contrário, você não consegue enviar este repositório para um repositório remoto_

**_Comandos Git:_**

* _git add *_ (pega tudo o que foi modificado e adiciona para a _staging area_, para a gente poder commitar)
* **git commit -m "commit inicial"**
* **git status** (vai ajudar a monitorar os status dos arquivos)



### Passo **6**

Criar uma pasta chamada **desafio-github** dentro da pasta **dio-desafio-github-primeiro-repositorio**

**_Comandos Git:_**

* **mkdir desafio-github**
* **mv Anotações.txt ./desafio-github/**



### Passo 7

Mover essas alterações que a gente fez para a _staging area_ e depois commitar esses arquivos

**_Comandos Git:_**

* **git add Anotações.txt desafio-github/**
* **git commit -m "cria pasta desafio-github, move arquivo para desafio-github"**



### Passo 8

Criar um arquivo Markdown (extensão .md) **README** dentro da pasta **dio-desafio-github-primeiro-repositorio**, para que sirva como uma espécie de _index_ (esse arquivo é o que as pessoas vão ver, com todos os passos que tem no nosso desafio) 

_Obs.: Se você quiser saber como o Markdown funciona, você pode vir aqui: [Sintaxe Básica Markdown](https://www.markdownguide.org/basic-syntax/)_

**_Comandos Git:_**

* **echo > README.md**



### Passo 9

Abrir o arquivo README.md no Typora e digitar o passo-a-passo, que será a "capa" do nosso Desafio de Projeto

**_Comandos Git:_**

* _git add *_
* **git commit -m "adiciona index"**



### Passo 10

Criar uma conta no GitHub

Entrar nos seus repositórios e clicar no botão "New"

Criar o nome do seu repositório (**Repository name:** dio-desafio-github-primeiro-repositorio)

Adicionar uma descrição (**Description**: Desafio de Projeto sobre Git/GitHub da DIO)

Deixar o seu repositório **público**

Não marcar o _checkbox_ para inicializar o repositório com o README, porque, nesse caso, a gente já colocou um README no seu repositório local 

Clicar em **Create repository**

Com o nosso repositório criado, a gente tem que ir lá no nosso repositório local e apontar o nosso repositório local para o nosso repositório do GitHub. O endereço desse repositório no GitHub é uma url

Copiar esse caminho, abrir o Git Bash e empurrar a versão do nosso repositório local para o repositório remoto

**_Comandos Git:_**

* **git remote add origin https://github.com/manoela-moyses/Desafio-de-Projeto-sobre-Git-GitHub-da-DIO.git**
* **git push origin master** (leva o nosso código do nosso repositório local para o nosso repositório remoto)
