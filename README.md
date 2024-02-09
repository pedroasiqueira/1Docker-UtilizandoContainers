# 1Docker-UtilizandoContainers
# Dia 01: Utiliznado Containers - Docker

Docker nada mais é do que uma plataforma que possibilita o empacotamento de uma aplicação dentro de um contêiner. A partir desse momento, um software consegue se adequar e rodar em qualquer máquina que tenha essa tecnologia instalada.



Imagem vs Containers

A imagem é a nossa aplicação “empacotada” com todas as dependências necessárias já instaladas dentro dela.

Imagine a imagem Docker como um arquivo zip, que contém o código-fonte e tudo o que é necessário para a execução correta do projeto.
Não é possível entrar no “terminal” de uma imagem, já que ela não está em execução.
O Docker possui um arquivo especial chamado Dockerfile, que nos ajuda a criar imagens. Falaremos mais sobre isso adiante!

O container é um processo que representa a execução de uma imagem já construída anteriormente.

Imagine o container Docker como um programa que você executa após “descompactá-lo” de um arquivo zipado, que já veio com todas as dependências necessárias.
Apesar de ser um processo isolado, é possível entrar no terminal dentro do container!
É possível parar e continuar a execução de um container sem precisar recriá-lo.


Registry
- local remoto onde podemos enviar e baixar imagens Docker (gitHub do Docker?)
- feito para pegarmos imagens já prontas e não "perder tempo" criando do zero




Resumo da trybe:

Docker: conjunto de ferramentas (Daemon, API, CLI) para gerenciar imagens e containers.

Arquivo Dockerfile: arquivo com linguagem própria, com os passos necessários para criar uma nova imagem Docker usando o código-fonte de um projeto.

Imagem Docker: é o projeto “compactado”, que foi construído de acordo com os passos contidos no arquivo Dockerfile. Pode ser usado como base para criar novas imagens Docker.

Container: é a execução de projeto através da sua imagem Docker já construída anteriormente.

Registry: é o local remoto onde podemos enviar e baixar imagens Docker. Um registry pode ser público ou privado.

Docker Hub:

É o registry oficial da empresa Docker Inc.
Ele é público, porém possui alguns limites.
É possível assinar o serviço para utilizá-lo como registry privado.

`docker container run <flags>? <imagem>:<tag> <argumentos>?`