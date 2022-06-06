Solução Orquestradora v.2
==========

.. autosummary::
  
Method: users.getProfile
========================

Gets the current user's Gmail profile.

HTTP request
------------

.. code-block::
  
  GET https://gmail.googleapis.com/gmail/v1/users/{userId}/profile
  
Path parameters
---------------

====== =================
Parameters     
------------------------
userId string
        The user's email address. The special value can be used to indicate the authenticated user.me
====== =================


====== =================
Parameters     
------------------------
userId string
        The user's email address. The special value can be used to indicate the authenticated user.me
====== =================
False  False  False
True   False  True
False  True   True
True   True   True
====== =================


+------------------------+------------+----------+----------+
| Header row, column 1                                      |
+========================+============+==========+==========+
| body row 1, column 1   | column 2   | column 3 | column 4 |
+------------------------+------------+----------+----------+
| body row 2             | ...        | ...      |          |
+------------------------+------------+----------+----------+
