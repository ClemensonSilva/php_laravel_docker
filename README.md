# laravel-docker-enviroment

## Instalação 
- Rode os comandos
  
```sudo docker compose build ```

e

``` sudo docker compose up```

Após isso, abra um novo terminal no mesmo diretório do projeto e copie o comando

``` sudo docker compose exec php bash ```

ao entrar dentro do container php, rode os comandos nessa ordem: 

```composer update```

```cp .env.example .env```


```chmod -R 777 storage bootstrap/cache```

OBS: dá acesso ao storage

```php artisan migrate``` 
e
```php artisan key:generate```

após isso, basta ir até o http://localhost:8088/  .
