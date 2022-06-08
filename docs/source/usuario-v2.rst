Usuário v.2
=========================

Overview
--------

Recurso
~~~~~~~

Não há dados persistentes associados a esse recurso.

+-------------+--------------------------------------------------------------------------------------------+
| Métodos     |                                                                                            |
+=============+============================================================================================+
| getProfile  | Obtém o perfil do Usuário atual no Gmail.                                                  |
+-------------+--------------------------------------------------------------------------------------------+
| stop        | Pare de receber notificações push para a caixa de correio do usuário dada.                 |
+-------------+--------------------------------------------------------------------------------------------+
| watch       | Configure ou atualize um relógio de notificação push na caixa de correio do usuário dada.  |
+-------------+--------------------------------------------------------------------------------------------+

Obter Profile
-------------

Obtém o perfil do Usuário atual no Gmail.

**Solicitação HTT**

.. code-block::
  
  GET https://gmail.googleapis.com/gmail/v1/users/{userId}/profile 

**Parâmetros de caminho**

============= ========= ========================================================================================================= 
  Parâmetros    Tipo      Descrição                                                                                                
============= ========= ========================================================================================================= 
  userId        string    O endereço de e-mail do usuário. O valor especial pode ser usado para indicar o usuário autenticado.me   
============= ========= ========================================================================================================= 

+---------------+---------+--------------------------------------------------------------------------------------------------------+ 
| Campos        | Tipo    | Descrição                                                                                              | 
+===============+=========+========================================================================================================+ 
| emailAddress  | string  | O endereço de e-mail do usuário.                                                                       | 
+---------------+---------+--------------------------------------------------------------------------------------------------------+ 
| messagesTotal | integer | O número total de mensagens na caixa de correio.                                                       | 
+---------------+---------+--------------------------------------------------------------------------------------------------------+ 
| threadsTotal  | integer | O número total de threads na caixa de correio.                                                         | 
+---------------+---------+--------------------------------------------------------------------------------------------------------+ 
| historyId     | string  | A ID do histórico atual da caixa de correio.                                                           | 
+---------------+---------+--------------------------------------------------------------------------------------------------------+

**Request body**

O corpo de solicitação deve estar vazio.

**Response body**

Se for bem sucedido, o corpo de resposta contém dados com a seguinte estrutura:

Perfil para um usuário do Gmail.

.. code-block:: js

  JSON representation

  {
    "emailAddress": string,
    "messagesTotal": integer,
    "threadsTotal": integer,
    "historyId": string
  }


+---------------+---------+--------------------------------------------------------------------------------------------------------+
| Campos        | Tipo    | Descrição                                                                                              |
+===============+=========+========================================================================================================+
| emailAddress  | string  | O endereço de e-mail do usuário.                                                                       |
+---------------+---------+--------------------------------------------------------------------------------------------------------+
| messagesTotal | integer | O número total de mensagens na caixa de correio.                                                       |
+---------------+---------+--------------------------------------------------------------------------------------------------------+
| threadsTotal  | integer | O número total de threads na caixa de correio.                                                         |
+---------------+---------+--------------------------------------------------------------------------------------------------------+
| historyId     | string  | A ID do histórico atual da caixa de correio.                                                           |
+---------------+---------+--------------------------------------------------------------------------------------------------------+

`Referência <https://developers.google.com/gmail/api/reference/rest/v1/users/getProfile>`_
