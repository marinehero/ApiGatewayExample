# Ocelot API Gateway example

>This sample shows how to use Ocelot API gateway to manage 2 services.

## Quick Overview

Structure

Directory |      | Port| path
----------|------|-----|------
|ApiGatewayExample/
||GatewayApi/  | 7000    | localhost:7000/catalog-api/currencies
||             |         | localhost:7000/orders-api/orders
||CatalogApi/  | 7001    | localhost:7001/api/currencies
||OrdersApi/   | 7002    | localhost:7002/api/orders

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
