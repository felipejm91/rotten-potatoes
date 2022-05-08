# rotten-potatoes

## Configuração

MONGODB_DB => Nome do database

MONGODB_HOST => Host do MongoDB

MONGODB_PORT => Posta de acesso ao MongoDB

MONGODB_USERNAME => Usuário do MongoDB

MONGODB_PASSWORD => Senha do MongoDB


=-*=-*=-*=-*=-*=-*=-*=-*=-*=-*=-*=-*=-*=-*=-*=-*=-*=-*=-*=-*=-*=-*=-*=-*=-*=-*=-*=-*=-*=-*=-*=-*=-*=-*=-*=-*=-*=-*=-*=-*=-*

PASSOS PARA CRIAÇÃO DA IMAGEM E EXECUÇÃO DOS CONTAINERS


1º) Criar o documento "Dockerfile" para documentar a criação da imagem da aplicação


2º)Executar comando para a criação da imagem, criando as versões seguindo as boas práticas

        docker build -t felipejm91/rotten-potatoes .

        docker build -t felipejm91/rotten-potatoes:v1 .


3º)Criar arquivo "docker-compose.yaml" para descrever como será a criação do ambiente, descrevendo cada container que irá fzer parte.


4º)Executar o comando para criação do ambiente com o docker-compose

        docker-compose up -d
    
4º)Acessar a aplicação


        Abrir um navegador e digitar o caminho "localhost:8080"


5º)Aplicação rodando em container
