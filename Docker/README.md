# Comandos Docker

Iniciar o docker ```sudo service docker start```

Criar um container ```docker run containerQueQuerCria```

Rodar container ```docker start nomeDoContainer```, ex: ```docker start postgres```

Parar container/image ```docker stop ID``` ou ```docker stop ImageName```

Excluir container ```docker rm ID ``` ou ```docker rm ImageName``` para excluir image

### PostgreSQL

```docker run --name nomeDoContainer -e POSTGRES_USER=user -e POSTGRES_PASSWORD=password -e POSTGRES_DB=nomeDoBanco -p porta:porta -d postgres```

**Exemplo:** ```docker run --name postgres -e POSTGRES_USER=root -e POSTGRES_PASSWORD=abobrinha -e POSTGRES_DB=testeDockerComPostgre -p 5432:5432 -d postgres```

### MySQL

```docker run --name nomeDoContainer -p porta:porta -e MYSQL_DATABASE=nomeDoBanco -e MYSQL_USER=user -e MYSQL_PASSWORD=password -d mysql:version```

**Exemplo:** ```docker run --name mysql -p 3306:3306 -e MYSQL_DATABASE=testeDockerComMySQL -e MYSQL_USER=root -e MYSQL_PASSWORD=abobrinha -d mysql:latest```
