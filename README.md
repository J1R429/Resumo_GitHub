<h1 align="center"> Resumo Estudo GitHub </h1> 

#Índice 🗃️
<u>* Introdução</u>
* [Definição](#Definição)
* Repositório
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









<h2></h2>
<h2></h2>
<h2></h2>








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




