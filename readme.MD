# Desafio de Engenheiro de software

## Observações: 
- [Vídeo do desafio](https://www.youtube.com/watch?v=e_WgAB0Th_I&list=WL&index=3)
- [Vídeo sobre micro serviços](https://www.youtube.com/watch?v=K1wPxx-YZyM&list=WL&index=6)

## Tecnologias utilizadas:

- Java 21
- Spring Boot
- Spring Data MongoDB
- RabbitMQ
- Docker

## Endpoints disponíveis: 

- http://localhost:8080/customers/{customerId}/orders

## Acessando o RabbitMQ: 

- http://localhost:15672

### Credênciais de acesso do RabbitMQ: 
- guest - para ambos os campos

### Exemplo de body para ser enviado do RabbitMQ:

```
   {
       "codigoPedido": 1001,
       "codigoCliente":1,
       "itens": [
           {
               "produto": "celular",
               "quantidade": 10,
               "preco": 1900.00
           },
           {
               "produto": "mouse",
               "quantidade": 100,
               "preco": 50.00
           }
       ]
   }
```