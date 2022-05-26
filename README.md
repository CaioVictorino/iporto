<p align="center"><a href="https://laravel.com" target="_blank"><img src="https://raw.githubusercontent.com/laravel/art/master/logo-lockup/5%20SVG/2%20CMYK/1%20Full%20Color/laravel-logolockup-cmyk-red.svg" width="400"></a></p>

<p align="center">
<a href="https://travis-ci.org/laravel/framework"><img src="https://travis-ci.org/laravel/framework.svg" alt="Build Status"></a>
<a href="https://packagist.org/packages/laravel/framework"><img src="https://img.shields.io/packagist/dt/laravel/framework" alt="Total Downloads"></a>
<a href="https://packagist.org/packages/laravel/framework"><img src="https://img.shields.io/packagist/v/laravel/framework" alt="Latest Stable Version"></a>
<a href="https://packagist.org/packages/laravel/framework"><img src="https://img.shields.io/packagist/l/laravel/framework" alt="License"></a>
</p>

## Requerimentos para o desenvolvimento

O projeto laravel foi criado utilizando composer, criando primeiramente os comandos e editando as descriptions e signatures dos comandos no App/Console/Commands.

Necessário requerir do composer o pacote guzzlehttp/guzzle através do comando "composer require guzzlehttp/guzzle", para consumo mais prático da API Binance.

Para o request funcionar corretamente é necessário configurar no php.ini o caminho para o arquivo cacert.pem, para nao retornar erro SSL no momento da requisição ao endpoint.

Criado model e migration para criar e consultar a base de dados.

Configurar o arquivo config/database.php, mude o valor do campo strict (do seu tipo de base de dados) para false.

Rota(s) de API consumida(s):
    
    Endpoint: https://testnet.binancefuture.com

    GET /fapi/v1/ticker/price
