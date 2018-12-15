# O que é `container` ?

Container é nada mais que um isolamento de recursos, que roda dentro de uma instancia, porém containers compartilham recursos do OS ao qual está sendo executado, diferente das maquinas virtuais, o contianer não precisa de recursos como kernel e driver, pense em um container como lojas de um shopping, cada loga tem sua propria caracteristicas e tamanho, mas todas compartilham os recursos do shopping em sí, todas estão detro da estrutura do shopping.

Sabendo desta informação vamos entender qual o papel do `Docker`

# O que é `Docker` ?

`Docker` é uma tecnologia que facilita manusear containers, com o docker você consegue realizar várias funcionalidades com containers de forma muito simples, para mais informações segue [link](https://docs.docker.com/)

![containers_docker](https://github.com/kaioaresi/docker/blob/master/Cap_1/imgs/containers_docker.png)

---

# Primeiros passo com `Docker`

## Instalando o docker
Existem alguns meios para realiza a instalanção do `docker`, se você é usuário linux, sua via é bem mais simples você poderá realizar a instalação via `curl`, gerenciado de pacote ou source, já se você é usuário windows até funciona mas eu **NÂO INDICO** por enguanto, existem site que você poderá trabalhar com docker sem muitos problemas, segue link:

- [Linux](https://docs.docker.com/install/linux/docker-ce/centos/)

Bom como falei acima para quem utiliza windows a melhor opção é criar um conta no docker hub e acessar o play with docker, que é uma plataforma gratuita já com docker instalado que lhe permite fazer teste com docker.

- [Play with docker](https://labs.play-with-docker.com/)


## Comandos básicos

Após realizar a instalação do docker, vamos checar as informações do mesmo, çomo estamos em 2018 é indicado que você utilize a versão do docker 18.+.


---
**Docker cli - Lógica de utilização**

Para utilizar o docker, primeiramento você deve conher sua logica de comandos, que é bem simple, ele utiliza o formato de subprocess, sequidos por parametros e cada comando possui seus respectivos parametros, vamos aos exemplos:

```
docker <comandos> <parametros>
```

Lista de todos subprocess (comandos).

```
docker container   Manage containers
docker image       Manage images
docker network     Manage networks
docker node        Manage Swarm nodes
docker plugin      Manage plugins
docker secret      Manage Docker secrets
docker service     Manage services
docker stack       Manage Docker stacks
docker swarm       Manage Swarm
docker system      Manage Docker
docker trust       Manage trust on Docker images
docker volume      Manage volumes
```

---

## Agora vamos a pratica

**Informações docker**

Aqui visualizamos todas as informações pertinentes ao docker, como versão, quantidade de imagens, containers e etc.

```
docker info
```

![Docker_info](https://github.com/kaioaresi/docker/blob/master/Cap_1/imgs/docker_info.png =300x450)


**Subindo um container**

Para que programa é um pratica muito comun na programação começarmos com o "Hello world", aqui não é diferente.

```
docker container run -ti hello-world
```
