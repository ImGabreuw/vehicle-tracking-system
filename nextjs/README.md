# Backend da interface de rastreamento - Next.js

Bem-vindo à documentação do backend da interface de rastreamento desenvolvido com Next.js. Este guia foi criado para fornecer informações abrangentes sobre como configurar, executar e testar a aplicação, além de destacar os pré-requisitos necessários para começar.

## Descrição

Este repositório contém o código-fonte do backend da interface de rastreamento desenvolvido utilizando a estrutura do Next.js. O backend é responsável por pré-renderizar ou renderizar a página web, além de realizar otimizações de performance (caching) e SEO.

## Pré-requisitos

Antes de começar, certifique-se de atender aos seguintes pré-requisitos:

- Docker e o plugin Compose instalados
- Node.js versão 20 ou superior

## Configurações

- Definir a variável de ambiente `GOOGLE_MAPS_API_KEY` no arquivo `.env` (a mesma utilizada pelo backend com Nest.js)

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
   ```

4. Ainda dentro do container Docker, inicie a aplicação com o comando:

   ```bash
   $ npm run dev
   ```

5. Acesse a aplicação através do navegador, visitando o endereço http://localhost:3001/new-routes ou http://localhost:3001/driver.

