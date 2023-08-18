# Sistemas de controle de versão:

Controla as versões de um arquivo ao longo do tempo

- Registra o histórico de atualizações de um arquivo;
- Gerencia quais foram as alterações, a data, o autor, etc;
- Organização, controle e segurança.

## Sistemas de controle de versão centralizado:

Existe apenas um servidor que vai conter as áreas de trabalhos conectadas a ele.

## Sistemas de controle de versão distribuído:

Clona o repositório completo, o que inclui o histórico de versões. Cada pessoa tem uma cópia do que está no servidor.

- Cada clone é como um backup
- Possibilita um fluxo de trabalho flexível
- Possibilidade de trabalhar sem conexão à rede

exemplo: Git.

## Git:

- Sistema de controle de versão distribuído.
- Gratuito e open-source
- Ramificações (branching) e fusões (merging) eficientes

🔗 _download:_ [Git - Download](https://git-scm.com/downloads)\
📖 _documentação:_ [Git - Reference](https://git-scm.com/docs)

### Fluxo básico do Git:

| git clone: clona um repositório Git existente para um novo diretório (pasta) local. |
|-|
| git commit: grava alterações no repositório |
| git pull: “puxa” as alterações do repositório remoto para o local (busca e mescla) |
| git push: “empurra” as alterações do repositório local para o remoto |

## GitHub:

Plataforma de hospedagem de código para controle de versão com Git, e colaboração.



### Criando e clonando repositórios:

Existem duas formas de obter um repositório Git na sua máquina:

    1. Transformando um diretório local que não está sob controle de versão, num repositório Git.
    2. Clonando um repositório Git existente.


**No Git Bash - Criando repositório local:**
| mkdir nomeDaPasta - cria pasta |
|-|
| cd nomeDaPasta - entra na pasta |
| cd .. - volta a pasta |
| git init - transforma a pasta num repositório git local |
| cd .git - mostra que é um diretório git |
| git clone linkDoRepositorioRemoto - clona o repositório remoto |
| git clone linkDoRepositorioRemoto |nome-do-diretorio-local - clona o repositório remoto e altera o nome |
| cat config - mostra o conteúdo do config da pasta |
| git remote -v - mostra os repositórios remotos que você está vinculado |
| git remote add origin linkDoRepositorioRemoto - |
| git clone linkDoRepositorioRemoto —branch feature-1 —single-branch: clona a branch pedida |
| ctrl + L: limpa o terminal |


**Criando novo repositório no GitHub:**

| git init |
|-|
| git add -a “first commit" |
| git branch -M main |
| git remote add origin linkDoRepositorio |
| git push -u origin main |


**Pegar um repositório existente e vincular:**


| git remote add origin linkDoRepositorio |
|-|
| git branch -M main |
| git push -u origin main |



**Outros comandos:**

| git status: mostra o status da árvore de preparação (staging area)  dos arquivos (se estava em um commit ou não) |
|-|
| git branch -M main |
| git push -u origin main |





