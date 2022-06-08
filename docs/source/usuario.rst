Usuário
=======

Overview
--------

"Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum."

Representação de recursos
-------------------------

A tabela a seguir mostra a lista de propriedades em um recurso do usuário.

+----------------+----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| Ação           | Solicitação HTTP                                                                                                                                                                 |
+================+==================================================================================================================================================================================+
| List users     | ``GET /usuários`` Recupera uma lista de usuários em seu sistema. Você pode consultar a lista usando vários parâmetros                                                            |
+----------------+----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| View a user    | ``GET /users/{user_id}`` Recupera informações de um usuário.                                                                                                                     |
+----------------+----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| Create a user  | ``POST /usuários``  Cria um novo usuário no aplicativo. Você pode optar por autenticar o usuário apenas com seu ID de usuário, ou com um token de acesso ou um token de sessão.  |
+----------------+----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| Update a user  | ``PUT /users/{user_id}``  Atualiza informações de um usuário.                                                                                                                    |
+----------------+----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+

Obter usuários
==============

Recupera uma lista de usuários. Você pode consultar a lista usando vários parâmetros.

.. code-block:: js
  
  Solicitação HTTP
  
  GET https://api-{application_id}.sendbird.com/v3/users
  
Parâmetros de caminho
---------------------

+-------------+---------+-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| Parâmetros  | Tipo    | Descrição                                                                                                                                                                                                 |
+=============+=========+===========================================================================================================================================================================================================+
| token       | string  | Especifica um token de página que indica o índice inicial de resultados a ser recuperado. Se não especificado, o índice está definido como 0                                                              |
+-------------+---------+-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| limit       | int     | Especifica o número de resultados a retornar por página. Os valores aceitáveis são de 1 a 100, inclusive. (Padrão: 10)                                                                                    |
+-------------+---------+-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| user_ids    | string  | Especifica as identidades do usuário. O valor deve ser uma sequência separada de círgula que consiste em múltiplos urlencoded IDs de usuário. O número máximo de IDs de usuário neste parâmetro é de 250  |
+-------------+---------+-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| nickname    | string  | Especifica os caracteres iniciais dos apelidos a procurar. Quando especificado, a solicitação de API procura usuários cujos apelidos começam com o valor especificado. Urlencoding recomenda-se o valor.  |
+-------------+---------+-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+

Request body
------------

O corpo de solicitação deve estar vazio.

Response body
-------------

Se for bem sucedido, o corpo de resposta contém dados com a seguinte estrutura:

.. code-block:: js
  
  {
    "user_id": "Craig",
    "nickname": "Shopperholic",
    "is_active": true,
    "is_online": true,
    "created_at": 1542123432,
  }
