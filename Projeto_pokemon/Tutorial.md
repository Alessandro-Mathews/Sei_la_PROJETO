**Como clonar o arquivo do repositório do GitHub em uma pasta, sem precisar baixar**

Opa, bem-vindo ao tutorial que mostra passo à passo como realizar o tratamento dos dados e fazer a ingestão dos dados no Mysql e no MongoDB. Antes de tudo, temos que clonar a pasta do GitHub no nosso computador. Caso não souber, segue a explicação:

-1 passo:Dentro do repositório do GitHub, clica no <>Code,  na cor verde, no Github. Após isso copia a URL do código, como demonstra a imagem abaixo:


-2 Feito isso, crie uma pasta com o nome que você desejar, no lugar onde você quer deixar o projeto. Vou criar uma na área de trabalho com o nome "Temp".

-3 Em seguida, abra a pasta com o nome que você escolheu, nesse caso: "Temp", selecione o diretório como na imagem abaixo e apague tudo. Em seguida digite o seguinte comando: git clone (LinkDoGitHub), para selecionar o link, basta apertar:  Ctrl+V, para colar o código do GitHub e depois aperte Enter. Automaticamente ele irá copiar todos os arquivos na pasta Temp. Segue o exemplo abaixo:


**Como executar o projeto no meu computador**

Primeiro passo, baixar o VsCode. Iremos precisar dele para baixar todas as bibliotecas necessárias para executar o código.
 Tem dois modos de inserir os dados, se você tiver o: Mysql e o MongoDB, os bancos de dados que iremos utilizar, basta executá-los, seguindo o passo à passo. Caso não, vai ser necessário fazer o uso do DOCKER, que está em outro arquivo. 

* Primeira parte: *como realizar o tratamento dos dados:*

Após clonar o GitHub no seu computador, e consequentemente ter o Vscode instalado, vocês irão abrir a pasta do "Sei_la_projeto", no Vscode e ele irá exibir todos os arquivos dentro dela. Após isso entrem na basta "Tratamento de da dados", depois em "scriptalteracaodetabela" é lá que iremos mexer e fazer nossas primeiras modificações no Dataset do Kaggle.
 O primeiro passo é baixar as extensões necessárias, nesse caso, ele irá pedir para baixar o Python para executar o código.


Bibliotecas que serão necessárias para executar o código:


Observação, para instalar as bibliotecas tem que ser pelo terminal, se tentar no código não irá funcionar. Para quem não sabe onde abrir o terminal:


1- Após realiar os downloads das bibliotecas necessárias, pode executar o código. Cada linha no código está com um -> "#" isso quer dizer que tem um comentário explicando o que cada comando faz, basta executar linha por linha, para isso:


* Segunda parte: *Como enviar os dados do Dataset para o MYSQL*

Primeiro passo, abrir a pasta "ingestaosimples", no explorer do Vscode. Após isso, vai ter um aquivo chamado: Ingest.ipynb, é lá que vai ocorrer todo o envio da "tabela", que chamamos de Dataframe, para ser mais específico. Para o Mysql, e como isso ocorre? segue o tutorial abaixo:

Ah, observação: Se você realizou o download das bibliotecas no tutorial acima, não precisa baixar de novo, basta apenas fazer o importe delas, para utilizar.

1-Com o mysql instalado, você irá precisar criar um "SCHEMA", como fazer isso: Basta clicar com o botão direito na parte escrita schema, no mysql e digitar o nome dele. Nesse caso: pokemon_bd


Com o schema criado, basta ir na Query e digitar o seguinte comando para utiliza-lo: use pokemon_db
Depois é só rodar, segue o exemplo a seguir:


Pronto, os demais comandos estão todos comentados da mesma formar, porém é necessário explicar como realizar a conexão com o MYSQL, então vamos seguir:

1-No código no Vscode tem uma pasta chamada: Insgest.ipynb é lá que vai ser realizado toda a conexão, que irá funcionar da seguinte maneira:  

