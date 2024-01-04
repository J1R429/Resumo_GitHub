CRIAR REPOSITÓRIO
    git add README.md
    git commit -m "first commit"
    git branch -M main
    git remote add origin URL_REMOTE
    git push -u origin main



PARA MANDAR ATUALIZAÇÃO
1-  git add . 

2- git commit -m "mensagem"

3 - git push origin <nome_branch>



<PARA O GIT SABER QUEM VC É>
    git config --local user.name "Seu nome aqui"
    git config --local user.email "seu@email.aqui"
<>

<SE TER O ERRO Message 'src refspec master does not match any' >
    VERIFICAR E VOLTAR AO PASSO DO COMMIT E SUA MENSAGEM
<>

<MUDAR O NOME DA BRANCH NO TERMINAL>
    Renomear o branch local usando o -m de move: git branch -m master main
    Subir para o repositório com o novo nome. E usei -u para indicar que é o upstream: git push -u origin main
<>

<GIT PUUL>
    git remote add origin REMOTE-URL
    git remote -v
    git pull
    git pull remote-url branch
<>

<QUANDO O REPOSITÓRIO LOCAL ESTA EM UNIDADE D>
    git config --global --add safe.directory D:/_CAMINHO PRO REPODITORIO LOCAL

<>