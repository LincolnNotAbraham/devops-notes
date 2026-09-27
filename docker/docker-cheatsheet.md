# Docker Cheatsheet

## Comandos Basicos

```bash
# Listar containers
docker ps -a

# Listar imagens
docker images

# Buildar imagem
docker build -t nome:tag .

# Rodar container
docker run -d -p 8080:80 nginx

# Logs
docker logs -f container_name

# Executar comando no container
docker exec -it container_name bash

# Limpar containers parados
docker container prune

# Limpar imagens nao usadas
docker image prune -a
```

## Docker Compose

```bash
# Subir todos os servicos
docker-compose up -d

# Parar todos
docker-compose down

# Ver logs
docker-compose logs -f

# Rebuildar
docker-compose up --build
```
