# FRONT - GESTOR DE CRISES

O projeto faz parte do início do aprendizado da linguagem Python , através da matéria **Desenvolvimento Full Stack Avançado** 

O objetivo é atender os requisitos necessário para entrega do MVP sugerido pela PUC-RIO.

---
## Como executar

Para executar o projeto é necessário realizar o download e abrir a página index.html em qualquer navegador.

---
## Como executar através do Docker

Certifique-se de ter o [Docker](https://docs.docker.com/engine/install/) instalado e em execução em sua máquina.

Navegue até o diretório que contém o Dockerfile e o requirements.txt no terminal.
Execute **como administrador** o seguinte comando para construir a imagem Docker:

```
$ docker build -t frontcrises .
```

Uma vez criada a imagem, para executar o container basta executar, **como administrador**, seguinte o comando:

```
$ docker run -it -p 8080:80 frontcrises
```

Uma vez executando, para acessar a API, basta abrir o [http://localhost:8080/](http://localhost:8080/) no navegador.



### Alguns comandos úteis do Docker

**Para verificar se a imagem foi criada** você pode executar o seguinte comando:

```
$ docker images
```

Caso queira **remover uma imagem**, basta executar o comando:
```
$ docker rmi <IMAGE ID>
```
Subistituindo o `IMAGE ID` pelo código da imagem

**Para verificar se o container está em exceução** você pode executar o seguinte comando:

```
$ docker container ls --all
```

 Caso queira **parar um conatiner**, basta executar o comando:
```
$ docker stop <CONTAINER ID>
```
Subistituindo o `CONTAINER ID` pelo ID do conatiner


 Caso queira **destruir um conatiner**, basta executar o comando:
```
$ docker rm <CONTAINER ID>
```
Para mais comandos, veja a [documentação do docker](https://docs.docker.com/engine/reference/run/).
