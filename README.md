Servidor IOT - Sprint 3

Integrante:
Guilherme Doretto Sobreiro - RM: 99674

Link do Vídeo: https://youtu.be/F-1JgkKrURY

# README - Internet of Things (IoT) Server Setup Guide

Este README fornecerá uma introdução ao conceito de Internet das Coisas (IoT) e um guia passo a passo para configurar um servidor IoT com uma máquina virtual Ubuntu e a ferramenta Postman.

## O que é IoT?

A Internet das Coisas (IoT) refere-se a uma rede de dispositivos físicos conectados à Internet que coletam e compartilham dados entre si. Esses dispositivos podem incluir sensores, câmeras, medidores, veículos e muito mais. O objetivo principal do IoT é automatizar processos, tomar decisões com base em dados em tempo real e melhorar a eficiência em diversas áreas, como residências, empresas, saúde e indústria.

## Configurando um Servidor IoT

Para configurar um servidor IoT, você precisará seguir estes passos:

### 1. Instalação de uma Máquina Virtual

1.1. Baixe e instale um software de virtualização, como o VirtualBox (https://www.virtualbox.org/) ou o VMware (https://www.vmware.com/).

1.2. Baixe uma imagem ISO do sistema operacional Ubuntu em https://ubuntu.com/download/server e siga as instruções para criar uma máquina virtual com o Ubuntu como sistema operacional convidado.

### 2. Configuração do Ubuntu

2.1. Inicie a máquina virtual e siga as instruções de instalação do Ubuntu.

2.2. Atualize o sistema com os seguintes comandos no terminal:

```
sudo apt update
sudo apt upgrade
```

## 3. Instalar o "ifconfig" para identificar o IP da máquina virtual
```
sudo apt-get install net-tools
ifconfig
```

3.1 Fazer a instalação do git
```
sudo apt install git
```

## 4. Instalação do Docker
4.1. Instale o Docker, que é uma plataforma para desenvolvimento, envio e execução de aplicativos em contêineres. Execute os seguintes comandos:
```
sudo apt install docker.io
```

## 5. Copiar os arquivos do repositório Fiware
```
git clone https://github.com/fabiocabrini/fiware
cd fiware
```

## 6. Rodar os containers
```
sudo docker compose up -d
sudo docker stats
```

## 7. Instalação do Postman

7.1. Baixe o Postman em https://www.postman.com/downloads/ e siga as instruções para instalar a versão adequada ao seu sistema operacional.

## 8. Configurando o Servidor IoT
8.1. Agora, você pode instalar e configurar os serviços IoT no seu servidor, como o Mosquitto (um broker MQTT) ou o Node-RED (uma plataforma de automação IoT).

8.2. Certifique-se de que sua máquina virtual está configurada para ter acesso à Internet, pois os dispositivos IoT precisarão se conectar a serviços externos para funcionar adequadamente.

## 9. Testando com o Postman
9.1. Abra o Postman e comece a criar solicitações HTTP ou MQTT para interagir com seus dispositivos IoT ou serviços IoT instalados no servidor.

9.2. Importe o arquivo .json

9.3. Entre na pasta "FIWARE"

9.4. Abra a pasta "IOT Agent MQTT"

9.5. Clique em "Health Check"

9.6. Coloque o IP da Máquina e Pronto.


Agora você tem um servidor IoT configurado em sua máquina virtual Ubuntu e a ferramenta Postman para testar e interagir com seus dispositivos IoT.
