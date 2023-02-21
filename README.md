
# O que é Docker

Docker é uma plataforma de virtualização de software que permite que aplicativos e serviços sejam executados em "containers".

Container são ambientes isolados e portáteis que contêm tudo o que um aplicativo precisa para ser executado, incluindo código, bibliotecas e dependências.

Docker compartilha o mesmo Kernel do sistema operacional, são executados em ambientes isolados mas ainda usam o Kernel para executar aplicativos, significando que são mais leves e mais rápidos que as VM's (Virtual Machines).

## O que é Kernel

É o componente cental do sistema operacional que atua como uma ponte entre o hardware do computador e os programas que rodam no sistema. Kernel é o primeiro programa que roda quando o computador é ligado, permanecendo em execução enquando o sistema operacional está em uso.

O docker funciona com base em imagens, e essas imagens são arquivos que contém todos os recursos necessários para criar um container.



# Comandos básicos





```bash
  docker ps  // lista todos os containers ativos
```

```bash
  docker ps -a // mostra todos os container (ativos ou não)
```

```bash
  docker run -d node // a flag -d faz rodar a imagem em segundo plano 
```

```bash
  docker stop "containerId" // para de executar o container que está em segundo plano 
```

```bash
  docker start "containerId" // iniciar novamente um container
```

```bash
  docker run -d -p 80:80 nginx // faz o nginx rodar na porta 80  
```


```bash
  --name "nomeDesejado" // colocar um nome em um container já criado
```

```bash
  docker logs "nomeContainer" // mostra cada acesso, mensagens de erro, inicilização...
```

```bash
  docker rm "nomeContainer" // remove um container alocado no computador
```

```bash
  docker rmi "nomeImagem" // remove imagem alocado no computador
```

```bash
  docker imagem ls // lista todas as imagens alocado no computador 
```

```bash
  docker -t "nomeImagem" . // cria um build de uma imagem docker no caminho atual 
```

```bash
  docker system prune // remove tudo que não está sendo usado
```


## Encontrar imagens 

Para nós baixarmos imagens docker já prontas, podemos acessar o docker hub, lá ja existem diversar imagem criadas pelas empresas oficiais.

Para acessar clique [AQUI](https://hub.docker.com) ou no link https://hub.docker.com

