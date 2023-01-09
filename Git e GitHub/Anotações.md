# Introdução ao Git e GitHub

# Git:

### Importância:

- **Versionamento de código (controle de versão)**
    - Armazenamento em nuvem
    - Trabalho em equipe
- ==**Git**==: criado por Linus Torvalds

- [Download do Git](https://git-scm.com/downloads)

### Comandos básicos para um bom desempenho no terminal:

- O **Git** é um **CLI (Comand Line Interface):** não tem interface gráfica. É feito por linha de comando.

**Windows**:

**Unix**:

**o que faz**

- cd + nome da pasta

- cd + nome da pasta

**c**hange **d**irectory

muda de diretório

ex: cd / (vai para a pasta raíz C)

- cd ..
- cd ..

volta um nível na navegação

- cd + tab

.

completa o nome da pasta

- cls
- clear ou ctrl+ L

limpa o terminal

- dir
- Is

lista os diretórios contidos na pasta 

- mkdir + nome da pasta
- mkdir + nome da pasta

cria um diretório

- del
- del

deleta um arquivo

- rmdir /S /Q
- rm -rf

deleta um diretório com todas as pastas dentro

- echo + texto
- echo + texto

printa o texto

- echo + texto > nome arquivo
- echo + texto > nome arquivo

cria um arquivo com esse nome

### Entendendo como o Git funciona por baixo dos panos:

- **SHA1**
    - SHA significa Secure Hash Algorithm (algoritmo de hash seguro) — é um conjunto de funções hash criptográficas projetadas pela NSA (Agência de segurança nacional dos EUA)
        - a encriptação gera conjunto de caracteres identificador de 40 dígitos, o SHA1.
        
        ex: 02a8502b44a75bd4ef6679b0588f0ce315bfdd55
        
- **Objetos fundamentais**
    - **BLOBS**: tem o SHA1 do arquivo — o tipo do objeto, o tamanho, \0 e o conteúdo de fato.
    - **TREES**: armazenam e apontam para os BLOBS. Monta toda a estrutura de onde estão os arquivos. Também tem o SHA1 das árvores.
    - **COMMITS**: objeto que dá sentido à alteração.
        - Aponta para uma árvore, para o último commit realizado, para o autor e para a mensagem.
- **Sistema distribuído**
- **Segurança**


### Primeiros comandos com o Git:

- **git init** — inicializa repositório no git
- **git add** **nomeArquivo** — nomeia o arquivo
- **git add .** — adiciona arquivos novos e modificados
- **git add *** — adiciona arquivos novos e modificados do diretório atual
    - ex: git add *.java - adiciona todos os arquivos terminados com .java
- **git commit -m “mensagem”** — faz um commit
- **git status** — mostra se os arquivos sofreram edição e precisam ser movidos pro staged — para depois ir pro commit

![Untitled](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/a51c7fe2-ebee-4315-94a2-2a59774a7520/Untitled.png)

- **Ambiente de desenvolvimento**
    - Working directory
    - Staging Area
    - Local Repository

### Trabalhando com o Git e GitHub:

- **git clone** + link do repositorio — clona um repositório
- cria o repositório online no github
- Abre o Gitbash dentro da pasta que você quer adicionar ao repositório.
    - digita **git remote add origin + link do repositório**
    - digita **git remote -v** para listar o que foi colocado
    - digita **git status** para ver se está na branch
    - digita **git push origin master** para dar um push e verificar a branch master.
    
- **ls -a** — mostra os diretórios ocutos
- **git remote -v** — mostra os repositórios remotos que o repositório baixado está apontado

### Resolvendo conflitos:

- ***git pull*** — traz o repositório remoto para o local, caso o remoto esteja com algo diferente