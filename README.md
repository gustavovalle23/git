# GIT E GITHUB

Guia Prático com base nos tutoriais da Rocketseat e blog.cedrotech
https://www.youtube.com/watch?v=2alg7MQ6_sI&vl=pt
https://blog.cedrotech.com/git-o-minimo-que-voce-precisa-saber-para-trabalhar-em-equipe/
https://blog.cedrotech.com/git-o-minimo-que-voce-precisa-saber-para-trabalhar-em-equipe-parte-2/

## Breve explicação
Esse repositório tem como objetivo tratar de maneira bem didática os conceitos e utilização do git. Para isso, em alguns momentos, será necessário usar palavras não muito corretas, mas para didática mais fácil e entendimento rápido.

O git é um sistema de controle de versões. Basicamente, você quer que o seu código esteja com muitos "backups" para caso você queira olhar, modificar ou desfazer algo que você já fez, é possível. 

### Repositório e Branch
Quando você cria um repositório, é algo como um projeto, uma pasta ou um sistema. Nele você pode colocar várias branchs. Uma branch é como se fosse uma linha do tempo. Imagina que você queira adicionar uma funcionalidade no seu código, mas isso pode acarretar em vários bugs e vai ser difícil e trabalhoso desfazer o que você fez. Simples, você cria uma branch. Criando essa linha do tempo, tudo que você fizer nela, fica nela (até você decidir juntar com a master). Caso você queira desfazer, é só mudar pra branch master novamente e sucesso.
### Commit
Porém, se você gostou da alteração que você fez, você pode dar um commit (confirmação de alteração). Você geralmente coloca uma mensagem pra falar o que você mudou ou o que adicionou para que você ou outros colaboradores possam entender o que foi feito naquela alteração. E se você quiser ver ou voltar para aquele momento daquela alteração, você pode também.


### Instalação

https://git-scm.com/download

### Comandos:
(esses comandos foram realizados no ambiente Linux, mas raramente serão diferentes no Windows)


- git init
    - Iniciar repositório naquele diretório (pasta)
- touch landingpage.html
    - Criar arquivo landingpage.html
- git add landingpage.html
    - Adicionar arquivo ao repositório local.
- git commit -m "added landing page"
    - Fazer commit com comentário. Cada commit vai ter um código, com 7bc79ed0ba4d516318b3545ab88822a7ee8bfb99 junto com o comentário
- git log
    - Ver logs dos commits (pontos na história do projeto)
- git status
    - Mostra o status de modificações feitas e os arquivos que não estão no histórico do git (arquivos não monitorados ou Untraked)
- git show 7bc79ed0ba4d516318b3545ab88822a7ee8bfb99
    - Mostra o que foi alterado naquele commit
- git show
    - Mostra o último ponto na história
- git branch featureNova
    - Criar linha do tempo alternativa
- git checkout featureNova
    - Mudar para linha do tempo alternativa
- git checkout master
    - Voltar para a linha do tempo principal
- git branch
    - Mostra todas as ramificações (linhas do tempo)
- git merge featureNova
    - Une a linha do tempo alternativa com a master
- git branch -D featureNova
    - Deleta a branch

- git add .
    - Adiciona tudo e todas as alterações da pasta
- git config credential.helper store
    - Autorizar push no github sem perguntar senha

- git remote add origin https://github.com/gustavovalle23/git.git
    - Inicializar repositório no Github após criá-lo no github
- git push -u origin master
    - Criar branch master

- git config credential.helper store
    - Armazena o login e senha

- git clone https://github.com/gustavovalle23/Agenda-em-C.git
    - Clonar o projeto para si na pasta atual

- git checkout -b teste
    - Criar a branch e mudar para ela

- git commit -am "update agenda.c"
    - Commit com add + mensage

- git pull
    - Atualizar repositório local com base no repositório remoto. Para casos de contribuições para o mesmo projeto
    
 - git push
    - Envia todas as alterações que você fez para o repositório remoto (github ou Bitbucket)


### Anotações
*   O git não pega todos os arquivos da pasta. Ele pega os arquivos que colocamos em observação com o 'git add'. E com o git commit ele pega esses arquivos e manda pro ponto da história

* Com o git log, ele mostra o commit com seu código. Copiamos esse código e colocamos no 'git show' com esse código


# SCENES

- [x] Você deseja criar pontos na história da produção do seu projeto
confirmações de alterações
- [x] Você deseja verificar mudanças feitas no seu projeto

- [x] Você começa uma nova funcionalidade no seu projeto, sem estragar o que já foi feito.

- [x] Você adiciona as novas funcionalidades ao seu projeto em produção

- [x] Você quer deletar a branch da nova funcionalidade, depois de aplicar em seu projeto.

- [x] Você quer colocar seu projeto na nuvem.

- [x] Você vai pegar um projeto já iniciado, para trabalhar com o time

- [x] Você precisa resolver um conflito.

- [x] Antes de enviar a resolução, precisamos atualizar o projeto local.

- [x] Você precisa voltar um arquivo para um determinado momento da linha do tempo.

- [x] Você precisa recuperar algo deletado.

*    git init // inicia a linha do tempo
*    git add // adiciona ou atualiza mudanças para irem para a linha do tempoo
*    git commit // adiciona um ponto na linha do tempo
*    git log // visualiza os pontos na linha do tempo / commit
*    git status // informa o estado das alterações do nosso projeto
*    git show // apresenta determinado ponto na história
*    git branch // gerenciar novas linhas do tempo
*    git checkout // manipula as linhas do tempo
*    git merge // unir linhas do tempo
*    git push // envia alterações locais para o repositório remoto
*    git clone // clonar um projeto / repositório
*    git pull // puxa do repositório remoto
