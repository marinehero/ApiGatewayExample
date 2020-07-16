# Ocelot API Gateway example

>This sample shows how to use Ocelot API gateway to manage 2 services.

## Quick Overview

Structure

ApiGatewayExample/
     GatewayApi/    serves on port 7000 /catalog-api/* & /orders-api/*
     CatalogApi/    on port 7001        /api/currencies
     OrdersApi/     on port 7002        /api/orders

``` bash
# install dependencies
cd CatalogApi
dotnet run
cd ../OrdersApi/
dotnet run

# serve with hot reload at localhost:7000 (with rate-limiting)
cd ../GatewayApi
dotnet run
```

## About Ocelot

Refer [Ocelot is a .NET API Gateway. This project is aimed at people using .NET running a micro services / service oriented architecture that need a unified point of entry into their system. However it will work with anything that speaks HTTP and run on any platform that ASP.NET Core supports](https://github.com/ThreeMammals/Ocelot)

For a documentation, please see [Big Picture](https://ocelot.readthedocs.io/en/latest/).
