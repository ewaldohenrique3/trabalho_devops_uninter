# Projeto Prático: DevOps e Integração Contínua (UNINTER)

[![Status](https://img.shields.io/badge/Status-Concluído-success)](https://github.com/ewaldohenrique3/trabalho_devops_uninter)
[![License](https://img.shields.io/badge/License-MIT-blue)](LICENSE)
[![Docker](https://img.shields.io/badge/Docker-Container-blue)](https://www.docker.com/)
[![CI/CD](https://img.shields.io/badge/CI%2FCD-GitHub%20Actions-orange)](https://github.com/features/actions)

---

## Descrição do Projeto
Este repositório contém a implementação do projeto prático da disciplina de **DevOps e Integração Contínua (UNINTER)**. O projeto consiste no desenvolvimento e entrega de um site estático para a empresa fictícia **CodeFactory Solutions**, aplicando boas práticas de versionamento de código com Git, containerização utilizando Docker e automação de fluxos de Integração Contínua (CI/CD) com GitHub Actions.

Link do repositório remoto: [https://github.com/ewaldohenrique3/trabalho_devops_uninter](https://github.com/ewaldohenrique3/trabalho_devops_uninter)

## Objetivo
O objetivo principal deste trabalho é demonstrar a aplicação prática dos conceitos de DevOps, garantindo:
* A padronização e portabilidade do ambiente de execução por meio de containers Docker.
* A automação do pipeline de build e testes utilizando GitHub Actions (`CI/CD`).
* A organização estruturada de um repositório remoto para documentação e entrega acadêmica.

## Tecnologias Utilizadas
As seguintes ferramentas e tecnologias foram empregadas no desenvolvimento do projeto:
* **HTML5, CSS3 e JavaScript:** Tecnologias base para a construção das páginas web estáticas.
* **Git e GitHub:** Controle de versão e hospedagem do repositório remoto.
* **Docker:** Ferramenta de containerização para empacotar a aplicação e suas dependências.
* **Nginx:** Servidor web leve utilizado no Dockerfile para servir os arquivos estáticos.
* **GitHub Actions:** Motor de automação para a pipeline de CI/CD.

## Estrutura de Pastas

```text
trabalho_devops_uninter/
├── .github/
│   └── workflows/
│       └── pipeline.yml
├── public/
│   ├── css/
│   │   └── style.css
│   └── images/
│       ├── aramis.png
│       ├── athos.png
│       ├── css3_icon.png
│       ├── dartagnan.png
│       ├── espadas.png
│       ├── espadas2.jpg
│       ├── favicon.ico
│       ├── fundo.png
│       ├── fundo02.png
│       ├── fundo03.png
│       ├── github_logo.png
│       ├── html5_icon.png
│       ├── insta1.png
│       ├── js_icon.png
│       ├── logo.instagram-20px.png
│       ├── mosq01.png
│       ├── mosq02.png
│       └── porthos.png
├── index.html
├── info.html
├── integrantes.html
├── Dockerfile
├── LICENSE
└── README.md

## Instruções de Instalação
Para rodar o projeto em um computador totalmente novo após clonar o repositório, o processo é bem simples e rápido graças ao Docker, já que você não precisa instalar servidores Web nem configurar dependências manuais na máquina.

### Pré-requisitos na Nova Máquina
Antes de começar, garanta que o novo PC tenha apenas duas ferramentas instaladas:
* **Git** (para clonar o repositório)
* **Docker Desktop** (com suporte a containers em execução)

### Clonar o Repositório
Abra o terminal (Prompt de Comando, PowerShell ou Git Bash) e execute:

git clone https://github.com/ewaldohenrique3/trabalho_devops_uninter.git

Em seguida, entre na pasta do projeto:

cd trabalho_devops_uninter

## Instruções de Execução
Com o Docker Desktop aberto e rodando, execute no terminal dentro da pasta do projeto:

1. Construir a imagem Docker:
   docker build -t site-integrantes:v1 .

2. Iniciar o container mapeando a porta:
   docker run -d -p 8080:80 --name site-app site-integrantes:v1

3. Acessar a Aplicação:
   Abra o navegador no seu computador e acesse:
   http://localhost:8080/

   Seu site estático servido pelo Nginx dentro do container já estará no ar perfeitamente.

### Comandos Úteis para o Dia a Dia
* Ver se o container está rodando:
  docker ps
* Parar o container:
  docker stop site-app
* Remover o container para recriar:
  docker rm site-app

## Licença
Este projeto está sob a licença MIT. Consulte o arquivo LICENSE para mais detalhes.
