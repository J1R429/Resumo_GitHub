<h1 align="center"> Resumo Estudo GitHub </h1> 

#Índice 🗃️
<u>* Introdução</u>
* [Definição](#Definição)
* [Repositório](#Repositório)
* Iniciar e gerenciar um novo branch
* Fazer alterações em um arquivo e enviá-los por push para GitHub Enterprise Cloud como commits
* Bifurcar um repositório - FORK

<h2>DEFINIÇÃO</h2>
- GIT: sistema de controle de versão distribuído e de código aberto <br /> 
- GITHUB: serviço de hospedagem para desenvolvimento de software e controle de versão <br /> 
__________

<h2>Repositório</h2>
Um repositório geralmente é usado para organizar um único projeto. Os repositórios podem conter pastas e arquivos, imagens, vídeos, planilhas e conjuntos de dados - tudo o que seu projeto precisar. 
__________

<h2>Iniciar e gerenciar um novo branch</h2>
O Branch permite que você tenha diferentes versões de um repositório de uma só vez.
Você pode usar branches para ter diferentes versões de um projeto de uma só vez. Isso é útil quando você deseja adicionar novas funcionalidades a um projeto sem alterar a principal fonte de código
O trabalho feito em diferentes branches não aparecerá no branch principal até que você faça o <b>merge</b>.
Se outra pessoa fez alterações no branch main enquanto você estava trabalhando no seu branch, você pode efetuar <b>pull</b> dessas atualizações.
__________

<h2>Fazer alterações em um arquivo e enviá-los por push para GitHub como commits</h2>
Você pode fazer e salvar as alterações nos arquivos do seu repositório. Em GitHub, as alterações salvas são denominadas commits. Cada commit tem uma mensagem de commit associada, que é uma descrição que explica por que uma determinada alteração foi feita. 
__________

<h2>Bifurcar um repositório - FORK 🍴</h2>
Um fork é um novo repositório que compartilha configurações de código e visibilidade com o repositório "upstream" original.
Os forks geralmente são usados para iterar ideias ou alterações antes de serem propostas de volta para o repositório upstream, como em projetos código aberto ou quando um usuário não tem acesso de gravação ao repositório upstream. 

Com ele você pode:
- Propor mudanças no projeto de outra pessoa
- Usar o projeto de outra pessoa como ponto de partida para sua própria ideia

__________





<h2>CURIOSIDADES</h2>
HEAD: Estado atual do nosso código, ou seja, onde o Git os colocou
Working tree: Local onde os arquivos realmente estão sendo armazenados e editados
index: Local onde o Git armazena o que será commitado, ou seja, o local entre a working tree e o repositório Git em si.

<h2>GIT IGNORE</h2>
- criar um arquivo com o nome .gitignoore, dentro dele em cada linha colocar os nomes dos arquivos que você quer que o github ignore e não monitore o status



<h2>CRIAR PASTA PARA SERVIR COMO REPOSITÓRIO</h2>
1) Crie uma pasta nova em seu computador;

2) No terminal (ou Git Bash, no Windows) navegue até a pasta recém criada (utilize o comando cd para navegar entre pastas);

3) Execute o comando git init --bare;

OBS: Não se esqueça do parâmetro --bare. Caso tenha executado o comando init sem esse parâmetro, execute na sequência o seguinte comando: git config core.bare true.

4) Navegue até a pasta onde se encontra o seu projeto;

5) Execute o comando git remote add local {caminho}. Substitua {caminho} pelo caminho completo da pasta recém criada;

6) Crie uma nova pasta em seu computador, para representar o trabalho de outra pessoa;

7) No terminal (ou Git Bash, no Windows) navegue até a pasta recém criada;

8) Execute o comando git clone {caminho} projeto. Substitua {caminho} pelo caminho completo da pasta que criamos no primeiro passo;

9) Observe que o repositório clonado está vazio;

10) Acesse a pasta Projeto e execute o comando 'git remote rename origin local' para renomear o repositório local da outra pessoa de "origin" para "local";

11) Navegue até a pasta onde se encontra o seu projeto original;

12) Execute o comando git push local master para enviar as suas modificações para o seu servidor;

13) Navegue até a pasta criada no passo 6;

14) Execute o comando git pull local master para baixar as modificações;

15) Abra o seu navegador e acesse http://github.com/;

16) Crie uma conta;

17) Crie um novo repositório, clicando no símbolo de adição no canto superior direito;

18) No terminal (ou Git Bash, no Windows) adicione, ao seu projeto inicial, o repositório remoto recém criado (os comandos são mostrados pelo próprio GitHub);

19) Execute git push origin main para enviar as suas alterações para o repositório no GitHub.




<h2>CAUSAR E RESOLVER CONFLITO NA BRANCH</h2>
1) Execute o comando git branch e veja que apenas a branch master existe no seu repositório;

2) Execute o comando git branch titulo e logo após execute o comando git branch. Veja que uma nova branch foi criada;

3) Agora, para começar a trabalhar nesta branch, digite git checkout titulo;

4) Execute novamente git branch e confira que agora você está na branch chamado titulo;

5) Altere o título da página index.html para "Cursos de DevOps da Alura";

6) Adicione as alterações com git add index.html;

7) Faça o commit, com git commit -m "Alterando título da página";

8) Execute o comando git log e confira o novo commit;

9) Altere o título da página para "Lista de cursos de DevOps da Alura";

10) Repita os passos 6 e 7, para adicionar um novo commit, alterando a mensagem;

11) Repita o passo 8 para conferir o novo commit;

12) Execute o comando git checkout master para voltar à linha de desenvolvimento master;

13) Execute git log para conferir que os últimos dois commits não estão lá. Confira se o conteúdo do seu arquivo também voltou ao seu estado original;

14) Na pasta criada para representar o trabalho de outra pessoa na aula anterior:

Execute git checkout -b lista para criar uma nova branch, chamada lista e passar a trabalhar nela;
Adicione o curso de "Kubernetes" na lista;
Repita os passos 6 e 7 para adicionar um novo commit, alterando a mensagem;
Execute o comando git checkout master para voltar à linha de desenvolvimento master;
15) Volte para a pasta que representa o seu próprio trabalho;

16) Altere o nome do curso de Docker para "Docker: Criando containers sem dor de cabeça";

17) Repita os passos 6 e 7 para adicionar um novo commit, alterando a mensagem;

18) Execute o comando git merge titulo para trazer o trabalho feito na branch titulo para a branch master;

19) Execute o comando git log --graph para ver as linhas de desenvolvimento (branches);

20) Execute git checkout titulo para trabalhar na branch chamada titulo;

21) Altere o título para ter a palavra "Cursos" com letra maiúscula;

22) Repita os passos 6 e 7 para adicionar um novo commit, alterando a mensagem;

23) Execute o comando git checkout master para voltar à linha de desenvolvimento master;

24) Execute o comando git rebase titulo;

25) Execute o comando git log e confira que o commit foi adicionado antes do commit realizado diretamente na branch master;

26) Execute o comando git push local master para enviar suas alterações para o repositório remoto que criamos na última aula;

27) Na pasta criada para representar o trabalho de outra pessoa na aula anterior:

Execute o comando git pull local master para baixar as alterações que você já realizou;
Execute o comando git checkout lista para continuar trabalhando na lista de cursos;
Altere o nome do curso de Docker para "Curso de Docker: Criando containers sem dor de cabeça";
Repita os passos 6 e 7 para adicionar um novo commit, alterando a mensagem;
Execute o comando git checkout master para voltar à linha de desenvolvimento master;
Tente juntar seu trabalho com git merge lista;
Veja que há conflitos. Corrija-os, deixando apenas a linha com o nome correto do curso;
Execute o comando git add index.html para informar que os conflitos neste arquivo foram corrigidos;
Execute o comando git commit para que o Git finalize o merge;
Execute o comando git push local master para enviar as suas alterações;
28) Volte para a pasta que representa o seu próprio trabalho;

29) Altere o nome do curso de Vagrant para "Vagrant: Gerenciando máquinas virtuais";

30) Repita os passos 6 e 7 para adicionar um novo commit, alterando a mensagem;

31) Tente executar o comando git push local master. Veja a falha;

32) Execute o comando git pull local master para trazer as alterações da outra pessoa;

33) Agora sim, execute o comando git push local master para enviar as alterações.


<h2>TAG</h2>
Uma Tag no Git é uma referência estática a um ponto específico na história do seu repositório. Ela é usada para marcar commits importantes, como versões estáveis, marcos de desenvolvimento ou releases principais. Basicamente, uma Tag é uma forma de nomear um commit específico para que você possa referenciá-lo facilmente posteriormente.

<h2>RELEASE</h2>
Uma Release no GitHub é uma versão específica do seu projeto que é disponibilizada para download ou deploy. É uma forma de empacotar um conjunto de arquivos do seu repositório em um formato que possa ser facilmente distribuído. Uma Release geralmente contém arquivos compilados, binários, documentação ou qualquer outra coisa necessária para distribuir seu software.


<h2>FASES</h2>
![image](https://github.com/jessicacanela/Resumo_GitHub/assets/123896356/cee736e6-1bbd-436f-87ab-bade6d653c0b)




:construction: Projeto em construção :construction:

ntroduçao
Conta e perfil
Autenticaçao
Repositórios
Administradores da empresa
Cobrança e pagamentos
Polftica do Site
Organizações
Seguranga do codigo
solicitações de pull
Problemas do GitHub
GitHub Actions
GitHub Actions
GitHub Copilot
Codespaces do GitHub
Migrações
GitHub Packages
Pesquisar no GitHub
Aplicativos
Webhooks e eventos
API REST
API GraphQL
CLI GitHub
GitHub Discussions
GitHub Sponsors
Criar comunidades




