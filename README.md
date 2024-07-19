# E-commerce API

Este projeto é uma API que simula um sistema de e-commerce. A API permite criar rotas, integrar um banco de dados, implementar a autenticação do usuário e fornecer funcionalidades essenciais, como listar produtos, adicionar itens ao carrinho de compras e efetuar o checkout dos itens.

## Funcionalidades

- Listagem de produtos
- Adição de itens ao carrinho de compras
- Autenticação de usuário
- Checkout de itens no carrinho

## Tecnologias Utilizadas

- Python
- Flask
- SQLAlchemy (ou outro ORM de sua escolha)
- JWT (para autenticação)
- SQLite (ou outro banco de dados de sua escolha)

## Requisitos

- Python 3.x
- Virtualenv

## Instalação

1. Clone o repositório:
    ```bash
    git clone https://github.com/seu-usuario/ecommerce-api.git
    ```

2. Crie e ative um ambiente virtual:
    ```bash
    cd ecommerce-api
    python -m venv venv
    source venv/bin/activate # No Windows use `venv\Scripts\activate`
    ```

3. Instale as dependências:
    ```bash
    pip install -r requirements.txt
    ```

4. Configure o banco de dados:
    ```bash
    flask db init
    flask db migrate
    flask db upgrade
    ```

5. Inicie a aplicação:
    ```bash
    flask run
    ```

## Endpoints

### Produtos

- **GET /products**: Lista todos os produtos
- **POST /products**: Adiciona um novo produto (necessita autenticação)

### Carrinho de Compras

- **GET /cart**: Lista os itens no carrinho de compras (necessita autenticação)
- **POST /cart**: Adiciona um item ao carrinho de compras (necessita autenticação)

### Autenticação

- **POST /login**: Realiza login do usuário e retorna um token JWT

## Contribuição

Se você deseja contribuir com este projeto, sinta-se à vontade para abrir uma issue ou enviar um pull request.

