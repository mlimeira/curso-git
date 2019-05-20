Curso de git do PPGCC da UFAC.

Segundo commit

Terceiro commit

Enviando versões usando ssh

Trabalhando no branch master

Resolvemos o conflito com sucesso

-----***-----***---Colaboração Silvana---***-----***-----
O Git suporta a criação de múltiplas linhas de desenvolvimento e através da criação de branches. 
Uma branche é uma abstração construída pelo git para representar uma linha de desenvolvimento. 
Geralmente, várias branches são criadas em um projeto e cada uma está associada ao desenvolvimento 
de um trabalho específico que agrega algum valor ao projeto. 
Em algum momento, quando estes trabalhos forem finalizados e estiverem estáveis, eles 
serão integrados "de volta" ao ramo principal (MASTER) pelo uso do comando MERGE.
-----***-----***---Fim da colaboração da Silvana---***-----***-----

Colaboração Thales

O Git se popularizou fortemente nos últimos anos. Dificilmente iremos encontrar um desenvolvedor
que não use ou tenha usado o Git alguma vez na vida. De fato, versionar código transcendeu as boas
práticas, e passou a ser um aspecto fundamental para qualquer projeto de software.
O Git é um sistema completíssimo para controle de versão de forma distribuída. Ele permite inúmeras
estratégias de versionamento, e atualmente está integrado a uma infinidade de ferramentas relacionadas
a processos de desenvolvimento de software.

Mas será que usamos todo o potencial desse sistema? No dia a dia, estamos aproveitando os comandos e
opções que o Git possui nativamente para facilitar nossa vida?
Pois bem, nesse post vamos começar falando sobre cinco comandos que o Git oferece e que podem trazer algumas
facilidades consideráveis para o cotidiano de alguém que versiona código, são eles:

    Analisando diferenças: git diff
    Avaliando alterações: git log
    Visualizando objetos: git show
    Guardando alterações temporariamente: git stash
    Copiando e colando commits: git cherry-pick

fim colaboração Thales

> Incluído por Daniel para forçar conflito e merge recursivo.

# Criando uma nova chave SSH no Windows
Contribuição por [Daniel Silva](https://github.com/danielnsilva)

As chaves SSH facilitam a comunicação com o Github, evitando ter que ficar digitando usuário e senha a cada conexão com o repositório remoto. No Windows, é possível criar a chave SSH por meio do Git Bash.

1. Com o [Git](https://gitforwindows.org/) instalado, abra o Git Bash.
2. Execute o comando abaixo, subtituindo o e-mail:
```$ ssh-keygen -t rsa -b 4096 -C "seu_email@exemplo.com"```
3. Pressione ENTER para manter o nome e local padrão do arquivo.
4. Uma senha de segurança pode ser atribuída a chave SSH, mas será solicitada sempre que a chave for utlizada. Pressione ENTER para manter em branco.

Fonte: https://help.github.com/en/articles/generating-a-new-ssh-key-and-adding-it-to-the-ssh-agent#generating-a-new-ssh-key
***

*****************************Colaboração Bruno Selhorst****************************
#Fazendo um clone de um repositório existente do Git
Caso você queira copiar um repositório do Git que já existe o comando será "git clone"
Sendo assim, para que se faça o clone do Git é necessário que seja utilizado o comando "git clone [url]"
Ficando o código como abaixo

$ git clone https://github.com/mlimeira/curso-git.git

Sendo assim, esse arquivo cria um diretório chamado curso-git, inicializa um diretório .git dentro dele e obtém do dados do repositório,
caso queria clonar o repositório em um diretório diferente, é possível especificar esse diretório utilizando a opção abaxo:

$ git clone https://github.com/mlimeira/curso-git.git nomedodiretorio

Este comando mudará o nome do diretório alvo para nomedodiretorio.

Esse texto foi retirado do site https://git-scm.com/book/pt-br/v1/Git-Essencial-Obtendo-um-Reposit%C3%B3rio-Git e foi modificado
conforme a necessidade.
***********************************************************************************
Colaboração Sarah Soares

Explorando o comando de log do Git
Os registros do Git permitem que você revise e leia um histórico de tudo 
que acontece em um repositório. O histórico é construído usando 
git-loguma ferramenta simples com várias opções para exibir o histórico 
de confirmação.
O que há no Log?
Um log do Git é um registro em execução de confirmações. Um log completo 
possui as seguintes partes:

Um hash de confirmação (soma de verificação de SHA1 40 caracteres do 
conteúdo de confirmações). Por ser gerado com base no conteúdo de 
confirmação, ele é exclusivo.
Metadados do Autor de Confirmação: O nome e endereço de email do autor 
do commit.
Metadados da Data de Confirmação: Um registro de data e hora para a hora 
da confirmação
Commit title / message: A visão geral do commit conforme escrito na 
mensagem de commit.
Os logs do Git podem ser o que você quiser que eles sejam. Git-log 
oferece dezenas e dezenas de opções, mas vamos começar com o mais 
simples.
Fonte: https://mijingo.com/blog/understanding-git-log

Colaboração Marcio Pontes


Trabalhando com Remotos
Para ser capaz de colaborar com qualquer projeto no Git, você precisa 
saber como gerenciar seus repositórios remotos. Repositórios remotos são 
versões do seu projeto que estão hospedados na Internet ou em uma rede 
em algum lugar. Você pode ter vários deles, geralmente cada um é somente 
leitura ou leitura/escrita pra você. Colaborar com outros envolve 
gerenciar esses repositórios remotos e fazer o push e pull de dados 
neles quando você precisa compartilhar trabalho. Gerenciar repositórios 
remotos inclui saber como adicionar repositório remoto, remover remotos 
que não são mais válidos, gerenciar vários branches remotos e defini-los 
como monitorados ou não, e mais. Nesta seção, vamos cobrir essas 
habilidades de gerenciamento remoto.

Exibindo Seus Remotos
Para ver quais servidores remotos você configurou, você pode executar o 
comando git remote. Ele lista o nome de cada remoto que você 
especificou. Se você tiver clonado seu repositório, você deve pelo menos 
ver um chamado origin — esse é o nome padrão que o Git dá ao servidor de 
onde você fez o clone:

$ git clone git://github.com/schacon/ticgit.git
