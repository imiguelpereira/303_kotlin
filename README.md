# Projeto DS303 - Aplicativo de Geolocalização e QR Code

## Objetivos

O objetivo deste projeto é desenvolver um aplicativo Android em Kotlin que faça uso de todas as funcionalidades ensinadas no curso DS303. O aplicativo deve ser capaz de ler um QR Code, obter a posição geográfica do dispositivo, associar a foto tirada com um aluno do grupo e enviar esses dados para um servidor através de uma API REST. Além disso, o aplicativo deve ser capaz de listar locais armazenados na API e exibir as imagens associadas a eles.

## Descrição Detalhada

O aplicativo consiste em duas principais funcionalidades:

### Leitura de QR Code

- O aplicativo possui um leitor de QR Code que pode ser acionado para ler um código QR.
- O código QR indicará o tipo de foto que deve ser tirada naquele ponto.

### Geolocalização e Associação com Aluno

- Após ler o QR Code, o aplicativo obtém a posição geográfica do dispositivo (latitude e longitude) através do GPS.
- O usuário deve digitar o RA de um dos alunos do grupo no aplicativo.
- O aplicativo associa a foto tirada com o aluno e a localização geográfica.
- Em seguida, os dados são preparados para serem enviados para o servidor da API REST.

### Envio de Dados para a API REST

- O aplicativo realiza uma chamada de API REST do tipo POST para enviar os dados (foto, RA do aluno e localização) para o servidor.
- Os dados são armazenados no servidor para posterior consulta.

### Lista de Locais Armazenados na API

- O aplicativo possui uma segunda tela que permite ao usuário listar os locais armazenados na API REST (GET).
- Ao selecionar um local da lista, o aplicativo exibe a imagem associada a esse local.

## Instalação

Para executar o projeto, siga as etapas a seguir:

1. Clone o repositório:

```bash
git clone https://github.com/imiguelpereira/303_kotlin
cd 303_kotlin
