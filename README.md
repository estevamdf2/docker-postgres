### docker-postgresql

<h2> Configuração para iniciar um container do postgres com o docker-compose </h2>

Crie um arquivo chamado .env e insira suas configurações de acesso ao banco
<ul>
<li>DATABASE_NAME</li>
<li>DATABASE_USER</li>
<li>DATABASE_PASSWORD</li>
<li>DATABASE_PORT</li>
</ul>

depois de configurar o .env inclua ele no .gitignore para não inclui-lo em seu repositório.

## Executando a aplicação
Construir uma instancia do container e executa-la em background

```
$ docker-compose up -d

```

## Acessando a base via psql 

```
$ psql -h localhost -p 5432 -U user database;
```
