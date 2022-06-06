Solução Orquestradora v.2
=========================

.. autosummary::
  
Método: users.getProfile
========================

Obtém o perfil do Usuário atual no Gmail.

Solicitação HTT
---------------

.. code-block::
  
  GET https://gmail.googleapis.com/gmail/v1/users/{userId}/profile
  
Parâmetros de caminho
---------------------

====== =================
Parameters     
------------------------
userId string

       O endereço de e-mail do usuário. O valor especial pode ser usado para indicar o usuário autenticado.me
====== =================

Request body
------------

O corpo de solicitação deve estar vazio.

Response body
-------------

Se for bem sucedido, o corpo de resposta contém dados com a seguinte estrutura:

Perfil para um usuário do Gmail.

.. code-block::
