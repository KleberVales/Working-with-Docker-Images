# Working with Docker Images 🐳

Este repositório contém exemplos e explicações sobre como trabalhar com imagens Docker.
As imagens são a base dos containers e permitem empacotar aplicações junto com suas dependências para garantir portabilidade e consistência.

## 📌 O que você vai aprender

- Como listar e buscar imagens
- Como criar novas imagens
- Como remover imagens antigas
- Como versionar imagens
- Como publicar no Docker Hub

## 🔹 Comandos básicos

1. Listar imagens

```bash
docker images
```

2. Baixar imagem do Docker Hub

```bash

docker pull <nome-da-imagem>:<tag>
# Exemplo:
docker pull nginx:latest

```

3. Criar container a partir de uma imagem

```bash

docker run -d --name meu_nginx -p 8080:80 nginx

```

4. Criar imagem a partir de um Dockerfile

```bash

docker build -t minha-imagem:1.0 .

```

5. Marcar (taggear) uma imagem

```bash

docker tag minha-imagem:1.0 usuario/meu-repositorio:1.0

```

6. Publicar imagem no Docker Hub

```bash

docker login
docker push usuario/meu-repositorio:1.0

```

7. Remover imagens

```bash

docker rmi <id-ou-nome-da-imagem>

```

## 📂 Estrutura do Repositório


