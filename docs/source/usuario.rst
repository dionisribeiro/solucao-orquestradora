Usuário
=======

.. autosummary::
   :toctree: generated

Overview
--------

"Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum."

Representação de recursos
-------------------------

``GET /users/{user_id}`` A tabela a seguir mostra a lista de propriedades em um recurso do usuário.

+----------------+------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| Ação           | Solicitação HTTP                                                                                                                                                             |
+================+==============================================================================================================================================================================+
| List users     | **GET /usuários** Recupera uma lista de usuários em seu sistema. Você pode consultar a lista usando vários parâmetros                                                        |
+----------------+------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| View a user    | ``GET /users/{user_id}`` Recupera informações de um usuário.                                                                                                                 |
+----------------+------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| Create a user  | POST /usuários  Cria um novo usuário no aplicativo. Você pode optar por autenticar o usuário apenas com seu ID de usuário, ou com um token de acesso ou um token de sessão.  |
+----------------+------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| Update a user  | PUT /users/{user_id}  Atualiza informações de um usuário.                                                                                                                    |
+----------------+------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+

