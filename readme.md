# Rocketseat - Guia Estelar de Git

Neste curso iremos aprender sobre tudo que o Git oferece pelo _**Mayk Brito**_ da Rocketseat

>E se você precisar revisitar seu código de meses atrás?, o Git vai te ajudar a versionar seu código evitando perdas indesejadas de código

## Aula 01 - Abertura
Iremos aprender a como instalar ele, para que serve, como funciona e o porque é tão utilizado

## Aula 02 - Por que este curso
Precisamos realizar este curso para aprendemos como modificar algo sem perder o que tinha feito, salvar e arquivar o código, evitar que percamos nosso projeto ou até modificar ele voltando para oque era antes com extrema facilidade

## Aula 03 - Controle de Versão
O controle de versão ou também conhecido por Version Control System (VCS) cria um registro de alterações em um ou mais arquivos, também vamos conseguir comparar as versões, verificar quem criou aquela linha de comandos e muito mais

## Aula 04 - Tipos de controles de versão
Existe três tipos de controle de versão onde são os:
  * Sistemas locais: Que é quando temos o projeto salvo somente no nosso computador e para criar as versões criamos diversas cópias e renomeamos para algo que conseguimos identificar, este método faz o desenvolvedor ficar expostos a diversos erros irreversível

  * Sistemas centralizados: Temos como exemplo o CVS, Subversion e Perforce, ele deixam o projeto salvo em um servidor onde assim vários clientes conseguem usar ele, por muitos anos este foi o método mais utilizado, mais ele tem alguns problemas onde se o servidor cair os desenvolvedores não vão conseguir codar e ele fica salvo em somente um local ficando proposto a perca do mesmo

  * Sistemas distribuídos: Temos como exemplo o Git, Mercurial, Bazaar e Darcs, ele é o mais utilizado permitindo o controle de versão sem erros, permite que vários desenvolvedores utilize o sistema e a perca do projeto é muito baixa pois ele fica salvo em todas as maquinas que está sendo desenvolvido e temos também a opção de salvar na nuvem

## Aula 05 - O que é o git
O grande ponto forte dele é a criação de commit (Ponto na história), criar um ponto na história é pedir para o sistema criar uma lista com todas as alterações realizadas desde o último commit, essas alterações é tudo mesmo como criação, renomeação, alteração e exclusão

## Aula 06 - Instalando git no mac
O próprio do [Git](https://git-scm.com/downloads) mostra os passos necessário para realizar a instalação, usando o gerenciador de pacote é o método mais recomendado

Para verificar se a instalação aconteceu sem problema devemos abrir um novo terminal e digitar o comando abaixo, este comando vai retornar a versão se estiver funcionando corretamente
````
git --version
````

## Aula 07 - Instalando git no windows
A única coisa que muda do mac é tipo da maquina

## Aula 08 - Instalando git no linux
Para realizar a instalação neste tipo de sistema temos os mesmo passos

## Aula 09 - Configuração inicial
Devemos falar para o git quem somos informando por exemplo nosso nome e e-mail, para realizar isso devemos usar os seguintes comandos em um terminal
````
git config --global user.name "Deibson Cogo"
git config --global user.email deibsoncogo@outlook.com
````

Este e-mail precisa ser o mesmo do seu Github para evitar conflitos

## Aula 10 - Git help
Ao usar o comando abaixo receberemos dicas tudo que o git pode fazer
````
git help
````

## Aula 11 - Iniciando um repositório
Usamos o comando abaixo para iniciar um repositório
````
git init
````

## Aula 12 - O o git guarda o histórico do projeto
Os dados ficam salvo em uma pasta oculta chamada de **.git**, se excluirmos ela iremos perder todo nosso histórico, por este motivo devemos mandar nosso projeto para a nuvem

Para baixar este histório da nuvem devemos usar o comando abaixo
````
git clone URLDoProjeto
````

## Aula 13 - Git log
Com o comando ````git log```` conseguimos emitir um relatório que vai mostrar diversas informações importante dos commits realizado ate o momento
  * ID do commit
  * Nome do criador
  * E-mail do criado
  * Data e hora que foi criado
  * Descrição informado pelo dev

Podemos adicionar ````--oneline```` no final para mostra um resumo das informações

Para mostrar somente uma certa quantidade a partir dos últimos commits usamos no final ````-n NumeroDeCommits````

Para ativar um filtro de data usamos ````--since=Ano-Mes-Dia```` para exibir os commits emitido depois da data e ````--until=Ano-Mes-Dia```` para antes

Para filtrar por autor devemos usar ````--author````

E o mais importante de todos é o ````--grep="Texto"```` que permite buscar algo que contenha certo texto

## Aula 14 - O primeiro commit
Agora iremos realizar o primeiro commit onde primeiro de tudo devemos ter algo para registrar como a criação de um arquivo, alteração ou exclusão

Depois usamos o primeiro comando abaixo para selecionar todos os arquivo que sofreram uma modificação de depois criamos o commit onde todos devem conter uma descrição
````
git add .
git commit -m "Commit inicial"
````

## Aula 15 - Estágios do arquivo
Existe três status dos arquivos do git onde para iniciar o repositório precisamos deste comando
````
git init
````

  * **Working diretory** é o momento que o arquivo é criado, excluído ou alterado
  * **Stage area** é o momento que selecionamos os arquivos para criar o commit
  * **Local repository** são os arquivos depois da criação do commit

## Aula 16 - Git Workflow
O git vai salvar as alterações criando uma copia do arquivo original, assim conseguimos modificar os pontos da história mais não conseguimos ter o mesmo arquivo na mesma etapa

## Aula 17 - Hash SHA-1
O ID que é criado para cada commit automaticamente é baseado no **Hash SHA-1** onde ele possui 40 caracteres hexadecimal, mais para a formação dele é utilizado oque realizamos nos modificações como texto utilizado e quando ocorreu, não podemos alterar ou excluir um commit sem deixar um rastro na história pois o ID já existente é utilizado na criação do próximo

## Aula 18 - HEAD
O head vai aponta em qual parte da história estamos como commit e linha pois podemos alterar ele

## Aula 19 - Revisão prática
Nesta aula revisamos tudo que aprendemos até o momento

Também vimos que com o comando abaixo conseguimos remover um arquivo da seleção
````
git rm --cached file.txt
````

E com este comando conseguimos alterar a descrição do último commit
````
git commit --amend -m "Nova descrição"
````

## Aula 20 - Adicionando arquivos com git add
Devemos procurar criar commits pequenos para assim a descrição dele ser assertiva

## Aula 21 - Editando arquivos
Aprendemos que de uma criação para alteração de um arquivo a única coisa que muda é o que o status mostra, pois ele agrupa por tipo de evento

## Aula 22 - Modificações com git diff
Com o comando abaixo conseguimos fazer o terminal mostrar um histórico detalhado das alterações captada, ele trabalha por linhas
````
git diff
````

## Aula 23 - Git diff staged
Na última aula usamos o diff para mostrar as alterações que possuia os arquivos na área de trabalho, para mostrar as alterações dos arquivos selecionados devemos usar este comando
````
git diff --staged
````

## Aula 24 - Deletando arquivos
A exclusão de um arquivo pode ser manualmente, selecionando o arquivo e dele, ou usar o comando abaixo onde ele excluirá por permanente a adicionará a edição as edições
````
git rm file.txt
````

## Aula 25 - Renomeando arquivos
A renomeação de um arquivo manualmente vai gerar um conflito no git, ao fazer isso ele vai pensar que deletamos um arquivo e criamos outro, para corrigir temos que utilizar estes comandos
````
git rm file.txt
git add arquivo.txt
````

Ou realizamos a renomeação pelo comando de **mv** como abaixo
````
git mv file.txt arquivo.txt
````

## Aula 26 - Movendo arquivos
Também teremos o mesmo problema acima quando movermos um arquivo de local, e para evitar devemos usar o mesmo comando mais um pouco diferente
````
git mv arquivo.txt sub/arquivo.txt
````

## Aula 27 - Desfazendo modificações
Usando o **restore** neste formato iremos fazer o arquivo voltar até a última seleção
````
git restore readme.md
````

## Aula 28 - Trazendo de volta do staged
Agora se no comando **restore** adicionarmos **staged** iremos pegar o arquivo selecionado a fazer ele voltar até o seu último commit realizado, também podemos alterar o nome do arquivo por ponto para assim fazer todos os arquivos voltarem ao seu último commit
````
git restore --staged readme.md
````

## Aula 29 - Corrigindo o último commit
Como já falamos todo commit possui um ID que é formado baseando-se nas alterações existente no commit, então quando alterarmos o commit seu ID muda, quando criamos um novo commit ele utiliza o ID do commit anterior criando um vinculo

Podemos alterar um commit a qualquer momento da história mais por eles serem vinculados isso se tornar algo muito avançado e perigoso

Agora aprenderemos a utilizar o **amend** que permite refazer por completo o último commit, seria como pegar todas as alterações selecionadas e enviar para o último commit invés de criar um novo
````
git commit --amend -m "Nova descrição"
````

## Aula 30 - Recuperando arquivos
Para recuperar um arquivo podemos usar o comando abaixo onde precisamos informar o ID (Completo ou resumido) do commit e o nome do arquivo que desejamos
````
git checkout 2b4d61a36b4cc39c29e166b9ce20703609f8de14 -- file.txt
````

## Aula 31 - Removendo arquivos não rastreados
Para remover um arquivo que não está sendo rastreado por definitivo usamos o comando abaixo, trocando o **-f** por **-n** será exibido uma lista dos arquivo que serão excluídos
````
git clean -n
git clean -f
````

## Aula 32 - Revertendo um commit
Com este comando consegui fazer o projeto voltar na história, assim desfazendo todas as alterações dos últimos 5 commit e criando um novo commit para registrar este acontecimento
````
git revert HEAD~5
````

Ou podemos utilizar para ele trazer de volta todas as alterações registra em um certo commit
````
git revert 2b4d61a36b4cc39c29e166b9ce20703609f8de14
````

## Aula 33 - Iniciando um novo projeto
Nesta aula realizamos o download de um projeto pronto onde a partir dele iremos rever tudo que já foi ensinado e aprenderemos novos comandos

## Aula 34 - Adicionando e verificando alterações
Como já sabemos com o **diff** conseguimos criar uma lista das alterações realiza em um momento, mais conseguimo resumir esta lista adicionando alguns comandos
````
git diff --color-words
````

## Aula 35 - Staging e commits com atalho
Quando já temos arquivos que está sendo rastreado conseguimos realizar uma combinação de comandos assim ganhando tempo, um único comando que vai executar o **add** e o **commit**
````
git commit -am "Descrição do commit"
````

## Aula 36 - Ver modificações em diversos pontos da história
Conseguimos criar uma lista das modificações realizada em commit anterior com o comando abaixo, também, conseguimos criar uma lista resumida das alterações, também conseguimos especificar os arquivos que queremos ver
````
git show 1d6c53d
git show 1d6c53d --color-words
git show ef6bc97 -- src/views/*
````
 