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
