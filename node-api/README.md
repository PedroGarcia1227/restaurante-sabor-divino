# API Node.js para o Restaurante Sabor Divino

Esta API utiliza programação assíncrona, e fornece várias funcionalidades para gerenciar clientes, endereços, pedidos e itens de cardápio para o projeto Restaurante Sabor Divino.

## Estrutura:

O projeto está organizado da seguinte forma:
- `routes/`: Contém os arquivos de roteamento, os endpoints da api.
- `db/`: Contém os módulos para interação com o banco de dados.

### Endpoints

## Inserir Cliente
- **URL:** `/inserir-cliente`
- **Método:** `POST`
- **Descrição:** Insere um novo cliente.
- **Corpo da Requisição:**
    ```json
    {
        "nomeUsuario": "string",
        "senha": "string"
    }

## Validar Login
- **URL:** `/validar-login`
- **Método:** POST
- **Descrição:** Valida o login de um cliente.
- **Corpo da Requisição:**
    ```json
    {
        "nomeUsuario": "string",
        "senha": "string"
    }

## Inserir Endereço do Cliente
- **URL:** `/inserir-endereco-cliente`
- **Método:** POST
- **Descrição:** Insere um novo endereço para um cliente.
- **Corpo da Requisição:**
    ```json
    {
        "nomeUsuario": "string",
        "Endereco": "string",
        "CEP": "string"
    }

## Inserir Pedido
- **URL:** `/inserir-pedido`
- **Método:** POST
- **Descrição:** Insere um novo pedido para um cliente.
- **Corpo da Requisição:**
    ```json
    {
        "nomeUsuario": "string",
        "metodoPagamento": "string"
    }

## Inserir Item ao Pedido
- **URL:** `/inserir-item-pedido`
- **Método:** POST
- **Descrição:** Insere um novo item ao pedido de um cliente.
- **Corpo da Requisição:**
    ```json
    {
        "nomeUsuario": "string",
        "nomeItem": "string",
        "quantidade": "number"
    }

## Calcular e Inserir Preço Total
- **URL:** `/calcular-e-inserir-preco-total`
- **Método:** POST
- **Descrição:** Calcula e insere o preço total de um pedido.
- **Corpo da Requisição:**
    ```json
    {
        "nomeUsuario": "string"
    }

## Obter Histórico de Pedidos
- **URL:** `/historico-pedidos/:nomeUsuario`
- **Método:** GET
- **Descrição:** Retorna o histórico de pedidos de um cliente.
- **Resposta de Sucesso:**
    ```json
    [
        {
            "IdPedido": "number",
            "DataEhora": "string",
            "PrecoTotal": "number",
            "Itens": [
            {
                "NomeItem": "string",
                "Quantidade": "number"
            }
            ]
        }
    ]

## Obter Lanches
- **URL:** `/selectLanches`
- **Método:** GET
- **Descrição:** Retorna todos os lanches disponíveis.
- **Resposta de Sucesso:**
    ```json
    [
        {
            "NomeItem": "string",
            "Preco": "number"
        }
    ]

## Obter Bebidas
- **URL:** `/selectBebidas`
- **Método:** GET
- **Descrição:** Retorna todas as bebidas disponíveis.
- **Resposta de Sucesso:**
    ```json
    [
        {
            "NomeItem": "string",
            "Preco": "number"
        }
    ]

## Obter Sobremesas
- **URL:** `/selectSobremesas`
- **Método:** GET
- **Descrição:** Retorna todas as sobremesas disponíveis.
- **Resposta de Sucesso:**
    ```json
    [
        {
            "NomeItem": "string",
            "Preco": "number"
        }
    ]
