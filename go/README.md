# Microsserviço de frete

Bem-vindo à documentação do microsserviço desenvolvido em Go, responsável pelo processamento de rotas e notificação em tempo real da localização de cada rota. Este guia foi criado para oferecer informações abrangentes sobre a configuração, execução e testes do microsserviço, além de destacar os pré-requisitos necessários para começar.

## Descrição

Este repositório contém o código-fonte do microsserviço desenvolvido utilizando a linguagem de programação Go. O microsserviço é encarregado de processar e gerenciar as rotas, bem como de notificar em tempo real a localização de cada rota aos interessados.

## Pré-requisitos

Antes de começar, certifique-se de atender aos seguintes pré-requisitos:

- Go versão 1.20 ou superior instalado

## Configuração

## Executando a aplicação

Siga estas etapas para executar o microsserviço:

1. Abra um terminal e execute o seguinte comando para iniciar os containers Docker:

   ```bash
   $ docker compose up
   ```

2. Execute o seguinte comando para compilar e iniciar o microsserviço:

   ```bash
   $ go run main.go
   ```

3. O microsserviço estará rodando e pronto para receber e processar as rotas.
