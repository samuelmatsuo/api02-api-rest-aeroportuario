# API 02 - API REST com Aeroportuário

Integrantes: 
- Mateus Stangherlin
- Felipe Carli
- Samuel Matsuo

## Rotas da API

### Cadastrar Aeronave
- **Método:** POST
- **Endpoint:** /aeronaves/
- **Corpo da Requisição:** Objeto de aeronave
- **Código de Status de Sucesso:** 200 (OK)

### Listar Aeronaves
- **Método:** GET
- **Endpoint:** /aeronaves/
- **Parâmetros:** Nenhum
- **Código de Status de Sucesso:** 200 (OK)

### Registrar Saída de Aeronave
- **Método:** PUT
- **Endpoint:** /aeronaves/{aeronave_id}/sair/
- **Parâmetros:** ID da aeronave
- **Código de Status de Sucesso:** 200 (OK)

### Excluir Aeronave
- **Método:** DELETE
- **Endpoint:** /aeronaves/{aeronave_id}/excluir/
- **Parâmetros:** ID da aeronave
- **Código de Status de Sucesso:** 200 (OK)


## Dependências do projeto

```shell
poetry add fastapi
poetry add typing
poetry add pydanctic
poetry add datatime
```


## Iniciando o servidor HTTP

```shell
uvicorn src.server:app --reload
```

Caso queira subir sem carregar o shell, execute o comando abaixo:

```shell
poetry run uvicorn src.server:app --reload
```
