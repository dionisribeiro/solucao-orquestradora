Usuário
=======================================



Faça apenas uma chamada de API e obtenha todos os seus dados meteorológicos essenciais para um local específico com a nossa nova **API OpenWeather One Call 3.0.**

A API One Call fornece os seguintes dados meteorológicos para quaisquer coordenadas geográficas:

* Tempo atual
* Previsão de minutos para 1 hora
* Previsão horária para 48 horas
* Previsão diária para 8 dias
* Alertas meteorológicos nacionais
* Dados meteorológicos históricos para mais de 40 anos (desde 1º de janeiro de 1979)

Como fazer uma chamada de API
-----------------------------

**Chamada de API**

.. code-block::
   
   https://api.openweathermap.org/data/3.0/onecall?lat={lat}&lon={lon}&exclude={part}&appid={API key}
   

**Parâmetros**

   ``lat, lon`` *Obrigatório* Coordenadas geográficas (latitude, longitude)

   ``appid`` *Obrigatório* Sua chave de API exclusiva (você sempre pode encontrá-la na página da sua conta na aba "chave API")
   
   ``exclude`` *Opcional* Ao usar este parâmetro, você pode excluir algumas partes dos dados meteorológicos da resposta da API. Deve ser uma lista delimitada
   por vírgula (sem espaços).
   
   Valores disponíveis:
   
      * ``current``
      * ``minutely``
      * ``hourly``
      * ``daily``
      * ``alerts``
      
**Exemplo de chamada de API**

.. code-block::

   https://api.openweathermap.org/data/3.0/onecall?lat=33.44&lon=-94.04&exclude=hourly,daily&appid={API key}
   

   
   
   
   
