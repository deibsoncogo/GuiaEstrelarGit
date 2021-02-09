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
