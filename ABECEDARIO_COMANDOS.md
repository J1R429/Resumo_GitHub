 ¯\_(ツ)_/¯

A
GIT ADD <NOME DO ARQUIVO QUE QUER MANDAR>¬ MANDA OS ARQUIVOS PARA A AREA DE STATIN
git add . ¬ para não precisa colocar o nome de um arquivo em especifico colaca o <.>, assim tudo que foi ateradp irá subir, realizar o commit

B
git branch - M '<nome da branch>' ¬ para mudar de branch 
git branch <nome> ¬ cria a branch
git branch -list ¬ para ver as branchs existentes

C
GIT COMMIT --AMEND  ¬ alterar a mensagem do ultimo commit 
GIT COMMIT -m "<MENSAGEM DO COMMIT>" ¬ PARA REALIZAR COMMIT
git checkout -b "<nome da nova branch>" ¬ para criar uma nova branch
git checkout <nome da branch que quer ir> ¬ para mudar de branch
git checkout ¬ Para deixar o nosso código em determinado estado
git checkout --help ¬ em uma tradução livre é: "Atualizar os arquivos na working tree para ficarem na versão especificada. [...]". Basicamente, podemos deixar o nosso código no estado do último commit de uma branch, de um commit específico, ou mesmo tags (que veremos adiante).
cd <nome do arquiv> ¬ para entrar num arquivo especifico
cd .. ¬ para subir uma pasta
git clone <caminho url> ¬ criar uma cópia de um repositório remoto em um diretório da máquina.
git checkout ¬ nós desfazemos uma alteração que ainda não foi adicionada ao index ou stage, ou seja, antes do git add. (depois do add é reset, depois do commit é revert)

D
git diff ¬ é possível visualizarmos as mudanças realizadas em determinado código

E
F
G
H
I
GIT INIT ¬ INICIA UM REPOSITORIO FACIL
git init --bare ¬ designar a pasta para ser pura, ou seja, apenas guardar as alterações do codigo que estará em outra pasta (cria um repositório que não terá a working tree, ou seja, não conterá uma cópia dos nossos arquivos. Como o repositório servirá apenas como servidor, para que outros membros da equipe sincronizem seus trabalhos, poupamos espaço de armazenamento desta forma.)

J
K
L
git log ¬ É utilizado para ver o histórico de alterações do projeto
git log --graf ¬ mostrar as linhas de comando d desenvolvimento
ls ¬ listar os arquivos da pasta

M
git merge <nome da branch que quer juntar> ¬ para juntar duas branch, necessário estar na branch considerada principal, a outra irá sumir
mkdir <nome> ¬ cria uma nova pasta

N
O
P
git push -u origin main ¬ empurrão do repositorio remato para o repositorio do site, usado na primeira vez
git push origin main ¬ empurrão usado quando não é a primeira vez
git pull ¬ puxar o repositorio do site para a maquina

Q
R
GIT REFLOG  ¬ você vai ver uma lista de tudo o que fez
GIT RESET ¬ utilizar para recuperação (utilizado depois do comando add, para desfazer uma alteração, precisamos tirá-la deste estado) (antes do add é checkout, depois do commit é revert)
git remote add origin <link do repositorio> ¬ utilizar o inset para colar - pedir conexão do repositorio local com o do site, utilizado apenas na primeira vez
git remote ¬ lista repositorios remotos
git remote add ¬ adiciona repositorio remoto
git remote -v ¬ mostra o endereço do repositorio remoto
rebase ¬ diferente da marg que só altera a linha, neste comando a o transporte do codigo fazendo com que fique integrado 
git revert ¬ utilizar para recuperação, quando já foi entregue o comando do add e do commit (antes do add é checkout e depois do commit é reset)


S
GIT STATUS ¬ MOSTRA O STATUS DO DOCUMENTO
git stash ¬ para armazenar temporariamente algumas de nossas alterações.

T
U
V
X
Y
W
Z
