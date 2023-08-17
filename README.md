# drinks_back_python

Aplicação back-end para uma aplicação que trabalha com drinks, utilizando **Python** e **Django**. Nesta aplicação, são gerenciadas as informações de drinks, permitindo a criação, leitura, atualização e exclusão dos registros.

## Dados

Cada drink possui os seguintes campos: **name** e **description**.             

## Endpoints

Essa aplicação expõe uma API RESTful, com os seguintes end-points:

Endpoint                    | Método    | Descrição
--------------------------- | --------  |-------------------
drinks                      | GET       | Retorna um array com todos os drinks
drinks/(:num)               | GET       | Retorna um drink cujo id é (:num)
drinks                      | POST      | Cria um novo drink
drinks/(:num)               | PUT       | Atualiza drink cujo id é (:num)
drinks/(:num)               | DELETE    | Deleta drink cujo id é (:num)

## Instalação

1. Clone este repositório e, na pasta raiz, execute o seguinte comando para instalar as dependências necessárias do projeto:

    ```
    > pip install -r requirements.txt
    ```

2. Agora, basta você dar o seguinte comando para subir o servidor:

    ```
    > python manage.py runserver
    ```

## Melhorias

O sistema está realizando todas as operações propostas, porém existem algumas melhorias a serem implementadas.

* Adicionar autenticação
    * Atualmente qualquer usuário pode efetuar as chamadas na API, sem qualquer autenticação.
* Melhorar error handling quando o body da chamada não possui os campos esperados.
