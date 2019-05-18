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

1. Com o [Git](https://git-scm.com/download/win) instalado, abra o Git Bash.
2. Execute o comando abaixo, subtituindo o e-mail:
```$ ssh-keygen -t rsa -b 4096 -C "seu_email@exemplo.com"```
3. Pressione ENTER para manter o nome e local padrão do arquivo.
4. Uma senha de segurança pode ser atribuída a chave SSH, mas será solicitada sempre que a chave for utlizada. Pressione ENTER para manter em branco.

Fonte: https://help.github.com/en/articles/generating-a-new-ssh-key-and-adding-it-to-the-ssh-agent#generating-a-new-ssh-key
***
