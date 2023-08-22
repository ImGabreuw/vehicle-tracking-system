# Backend - Nest.js

Bem-vindo à documentação do backend desenvolvido com Nest.js. Este guia foi criado para fornecer informações abrangentes sobre como configurar, executar e testar o backend, além de destacar os pré-requisitos necessários para começar.

## Descrição

Este repositório contém o código-fonte do backend desenvolvido utilizando a estrutura do Nest.js. O backend é responsável por fornecer funcionalidades essenciais para a aplicação, como integração com a API do Google Maps e outras características importantes.

## Pré-requisitos

Antes de começar, certifique-se de atender aos seguintes pré-requisitos:

- Docker e o plugin Compose instalados
- Node.js versão 20 ou superior

## Configurações

### Configuração da API do Google Maps

Siga estas etapas para configurar a API do Google Maps:

1. Acesse o [Google Console](https://console.cloud.google.com/).
2. Crie um novo projeto clicando em "Novo Projeto".
3. No menu lateral, vá para a seção "APIs e serviços" e clique em "Ativar APIs e Serviços".
4. Pesquise e ative as seguintes APIs: "Maps JavaScript API", "Directions API" e "Places API".
5. Em seguida, acesse a aba "Credenciais" no menu lateral, clique em "Criar Credenciais" e escolha "Chave API". Copie a chave gerada e cole-a no arquivo `.env`, na variável `GOOGLE_MAPS_API_KEY`.

## Executando a aplicação

Siga estas etapas para executar a aplicação:

1. Abra um terminal e execute o seguinte comando para iniciar os containers Docker:

   ```bash
   $ docker compose up
   ```

2. Abra outro terminal e execute o seguinte comando para acessar o container Docker da aplicação:

   ```bash
   $ docker compose exec app bash
   ```

3. Dentro do container Docker, configure as dependências iniciais executando os comandos:

   ```bash
   $ npm install
   $ npx prisma generate
   ```

4. Ainda dentro do container Docker, inicie a aplicação com o comando:

   ```bash
   $ npm run start:dev
   ```

5. Acesse a aplicação através do navegador, visitando o endereço http://localhost:3000/routes.

## Testando a aplicação

Você pode testar a aplicação usando o arquivo `api.http` localizado na raiz do projeto Nest.js. Este arquivo foi configurado para ser usado com o plugin [REST Client](https://marketplace.visualstudio.com/items?itemName=humao.rest-client) do VSCode. Ao enviar solicitações através deste arquivo, o Nest.js processará as requisições e exibirá mensagens no console.
