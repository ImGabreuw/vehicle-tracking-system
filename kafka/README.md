# Sistema de Mensageria (Backend) - Apache Kafka

## Descrição

Este é o repositório dedicado ao Apache Kafka, que compõe a infraestrutura do backend do sistema de mensageria.

## Configuração

### Configuração do `/etc/hosts`

A comunicação entre as aplicações ocorre diretamente através da rede da máquina. Para possibilitar isso, é fundamental configurar um endereço que todos os containers Docker possam acessar.

Em sistemas Linux/UNIX:

```console
$ echo "127.0.0.1 host.docker.internal" >> /etc/hosts
```

Em sistemas Windows:

```console
$ echo "127.0.0.1 host.docker.internal" >> C:\Windows\system32\drivers\etc\hosts
```

Independentemente do sistema operacional, é necessário executar o programa de edição do arquivo _hosts_ como Administrador da máquina ou com privilégios de root.

## Executando a aplicação

Siga as etapas abaixo para rodar a aplicação:

1. Execute o comando:

   ```console
   docker-compose up
   ```

2. Quando desejar parar os containers do Kafka, lembre-se de executar o **docker-compose down** para limpar o armazenamento antes de rodar novamente o **docker-compose up**. Isso evitará erros durante a nova inicialização.
