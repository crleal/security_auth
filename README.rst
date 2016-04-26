Welcome to 
===========================

Linha de comando linux:

curl --data "username=admin&password=admin123" http://localhost:8000/rest-auth/login/

Retorno:
ok:
{"key":"b2239195ccda8a17b8ea562c5eb7053049401d70"}

Erro:
{"non_field_errors":["Impossível fazer login com as credenciais fornecidas."]}
