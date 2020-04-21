

## Treinamento para projetos GPDS

Este repositório oferece um treinamento básico das principais ferramentas que são utilizadas nas pesquisa realizadas no Grupo de Processamento Digital de Sinais (GPDS). O conteúdo pode (DEVE), ser usado para consulta e sempre melhorado, fique à vontade para fazer seu **pull request** com alterações, sugestões e etc.

### Sumário

 - [Comandos básicos para Linux](https://github.com/JoseRaimundo/treinamento_projeto_ecg_gpds#linux)
 - [Github](https://github.com/JoseRaimundo/treinamento_projeto_ecg_gpds#github)
 - [Python](https://github.com/JoseRaimundo/treinamento_projeto_ecg_gpds#python)
	 - [Instalação](https://github.com/JoseRaimundo/treinamento_projeto_ecg_gpds#instala%C3%A7%C3%A3o)
	 - [Estrutura de projeto](https://github.com/JoseRaimundo/treinamento_projeto_ecg_gpds#estrutura-de-pastas-de-projetos)

### Linux (Ubuntu)

Por que usar Linux? - Sistemas operacionais como o Ubuntu, Debian, Fedora e etc. Ajudam bastante para quem vai trabalhar com desenvolvimento, pois tem uma gama de ferramentas e conteúdo na internet que podem auxiliar no desenvolvimento de suas aplicações. Algumas vantagens:

 - Instaladores de pacotes (você não precisa se preocupar com configurar máquina, ou instalar alguma DLL).
 - Não existe virus para Sistemas operacionais Linux.
 - Maior controle de instalações e atualizações (você não é forçado a instalar updates)
 - Demanda menos recursos computacionais que os demais sistemas operacionais como Windows 10, ou outros.
 - Estável, tem menos chances de travar ou corromper algum arquivo.

#### Comandos básicos para Linux

Lista de comandos para usar no terminal linux. Para abrir o terminal **tecle** `ctrl + alt + t` e use os seguintes comandos.   

Listando conteúdo de uma pasta:
	
	ls

Comandos para entrar e sair de uma pasta, respectivamente:

	cd nome_da_pasta
	cd ..

Criando uma nova pasta:

	mkdir nome_da_nova_pasta

Criando um novo arquivo:

	touch nome_do_novo_arquivo

Deletando arquivo:

	rm -rf nome_do_arquivo

Renomeando arquivo:

	mv arquivo_antigo artigo_novo

Copiando arquivos:

	cp arquivo outra_pasta/arquivo_copia	

Ver o path em que você está:

	pwd

Instalação de algum programa:
	
	sudo apt-get install nome_do_programa

### Github

O Github é uma poderosa ferramenta para quem vai trabalhar com códigos e em equipe, pois permite controle eficiente de versões do código além de possibilitar um fluxo de trabalho distribuído e fluído entre integrantes da equipe de desenvolvimento.

#### Instalando Github

No Linux (Ubuntu), basta digitar a seguinte linha no terminal:

	sudo apt-get install git

No Windows , baixe o arquivo disponível no site [gitforwindows.org](https://gitforwindows.org/), e siga o passo a passo. [Neste link](https://woliveiras.com.br/posts/instalando-o-git-windows/), há um tutorial explicando cada passo.

#### Criando conta

Crie uma conta no [site github](https://github.com/), é fácil e só precisa de um email e senha. Você também já pode configurar sua máquina, no terminal digite os seguintes comandos:

	git config --global user.name "Seu nome aqui"
	git config --global user.email "seu_email_aqui@email.com"

#### Criando repositório

Um repositório é como uma pasta no Github, no qual você colocará todos os arquivos da sua aplicação, explicações, licença, documentação e etc. Você pode criar pelo termina, porém é mais prático utilizar o site. Após logar no site do Github, no canto superior direito, há um sinal de **+** (próxima imagem), basta selecionar a opção **Novo repositório**, o restante é intuitivo.



> Tente evitar espaços, utilize underline (**_**) para separar as palavras, ex: meu_repositorio, ou letras maiúsculas para começar uma nova palavra, ex: meuRepositorio

![criando repositório](https://raw.githubusercontent.com/JoseRaimundo/treinamento_projeto_ecg_gpds/master/img/novo_repositorio.png)


##### Branchs

#### Clonando repositório

#### Subindo alterações


#### Sincronizando alterações

#### Documentando no README

### Visual Studio Code

O VS é um dos melhores ambientes de desenvolvimento que há, pois apresenta uma interface simples e é relativamente simples quando comparado a outras alternativas mais complexas. Para instalar, baixe o instalado no site oficial [AQUI](https://code.visualstudio.com/download). Caso você esteja utilizando o Ubuntu (Linux), baixe o aquivo **.deb** e digite o seguinte comando na pasta onde o arquivo está:

	sudo dpkg -i nome_do_arquivo_baixado.deb

Se acontecer algum problema, digite o comando e, após o comando terminar, tente instalar o programa novamente:

	sudo apt-get install -f 
	

### Python

!IMPORTANTE: Esse é apenas um tutorial básico, com as ferramentas mais usadas, para mais aprofundamentos acesse as documentações de referência no final de cada explicação.

#### Instalação

Apesar de haver versões mais recentes, é recomendado que instale uma das versões 3.5 - 3.7 do Phyton, pois são mais estáveis e com maior compatibilidade com aplicações e bibliotecas.

Para instalar no Ubuntu, use os comandos:

	sudo apt-get install python3.6
	sudo apt-get install python3-pip

O **pip** é uma ferramenta do python que ajuda na instalação de bibliotecas. 
 
#### Estrutura de Pastas de Projetos

Antes de começar a "codar", é bom organizar bem suas pastas e arquivos, uma alternativa para estrutura de projeto pode ser da seguinte forma:

	PastaDoProjeto
	--- main.py
	--> src
		 |--- funcao1.py
		 |--- funcao2.py	
	--> dataset
		 |--- dados.csv
	--> output
		 |--- graficos.png
		 |--- log.txt
	--- README.md
	--- .gitignore

Explicando: 

 - A **PastaDoProjeto** é onde ficará tudo, também é a pasta que representará seu repositório no **github**.
 - **main.py** é o arquivo principal, que é executado antes de qualquer coisa.
 - Na pasta **src** fica o restante dos seus códigos: funções, classes, outras pastas.
 - Na pasta **dataset** fica seu banco de dados, arquivos do tipo xls, csv e etc. São os dados que sua aplicação irá usar.
 - Na pasta **output** fica as saídas do seu programa, gráficos, anotações de resultados, arquivos de relatórios (log) e etc.
 - Ainda dentro da pasta principal, temos o arquivo **README.md** que contém as instruções que irão aparecer no github.
 - No aquivo **.gitignore** você colocará os arquivos que não quer que vá para o github, ex. Arquivos muito grande, imagens, arquivos com senhas, rascunhos e etc.

Esta estrutura de pastas não é uma regra geral, porém ela é simples e bem clara, o que ajudará para que outros pesquisadores entendam melhor o seu código/programa.



#### Dicas de programação com python

Estas são dicas baseadas em códigos e repositórios profissionais, e livros de boas práticas de programação, porém não é uma regra geral.

##### Dicas de padronização

Padronize a nomenclatura de seu código, utilize letras maiúsculas ou underline para diferenciar as palavras que compões o nome das funções e variáveis.
Exemplo de variáveis:

    variavel_teste = 10
    variavelTest = 10


Exemplo de funções:

    def funcao_teste():
    def funcaoTeste():

Utilize nomes bem definidos e que representem bem o significado da variável ou da função. Exemplo:

Errado:

    a = b + c

Certo:

	soma = primeiro_termo + segundo_termo


##### Dicas de optimização de código

**#Dica1**: Use valores default (valores padrões) nos parâmetros das funções. Esses valores serão utilizados se você não especificar um valor para a variável, com isso você garante que a função será alimentada e também evita que você tenha que preencher sempre um parâmetros que se repete várias vezes. Exemplo:

    def escreveNumeros(primeiro = 1, segundo = 2):
	    print("Primeiro Número: ", primeiro)
		print("Segundo Número: ", segundo)

Agora se você chamar essa função sem passar nenhum argumento, os valores default serão utilizados.

    escreveNumeros()
    # Saída
    Primeiro Núemro: 1
    Segundo Número: 2

  Exemplo passando valores pela ordem:

    escreveNumeros(3, 4)
    # Saída
    Primeiro Núemro: 3
    Segundo Número: 4

  Exemplo passando valores pelo nome (note que mesmo com a posição trocada, os valores assumem o nome do parâmetro ao qual ele é atribuído):

    escreveNumeros(seundo = 3, primeiro = 4)
    # Saída
    Primeiro Núemro: 4
    Segundo Número: 3

**#Dica2**:

 Variáveis globais não são recomendadas, porém em situações em que elas são utilizadas em muitos lugares com o mesmo valores elas são úteis,  ou quando elas possuem valores constantes, pois reduz o tempo gasto para atualizar seu valor em caso de testes. Uma dica para definir uma constante, é utilizar todas as letras maiúsculas. Exemplo:

    PI = 3.14
    CONSTANTE_TESTE = 10
    MAX_NUMERO = 999999999

#### Numpy


#### Pandas
#### Plotagem

### Machine Learning
#### Sklearn
#### Tensorflow

### Desafios

#### Manipulação de Dados

   1. Crie uma estrutura de pastas conforme explicado [aqui](https://github.com/JoseRaimundo/treinamento_projeto_ecg_gpds#estrutura-de-pastas-de-projetos).
   2. Dentro da pasta **dataset**, adicione esse banco de dados: Banco
   3. Crie uma função chamada **dataAnalise** que recebe um **dataframe** pandas e printa no terminal os titulos das colunas, dra
   4. Crie dois vetores, um para as features e outro para a classe.
      
### Utilidades

#### Links

 - [Deepleaning book - Enciclopédia online de Deep
   Learning](http://deeplearningbook.com.br/)
 - [Datascience Pizza - Repositório com vários dataset e conteúdos
   interessantes](https://github.com/PizzaDeDados/datascience-pizza)
 - [Machine learning mastery - Coleção de tutoriais bem explicados
   (Python)](https://machinelearningmastery.com/start-here/#getstarted)

#### Cursos 
 - [Cursera - Um dos melhores cursos gratuitous que existe sobre machine learning](https://pt.coursera.org/learn/machine-learning)

#### Vídeos

 - [StatQuest - Canal sobre machine learning com vídeos muito didáticos](https://www.youtube.com/user/joshstarmer)
