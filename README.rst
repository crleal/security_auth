Welcome to
===========================

Linha de comando linux:

curl --data "username=admin&password=admin123" http://localhost:8000/rest-auth/login/

Retorno:
ok:
{"key":"b2239195ccda8a17b8ea562c5eb7053049401d70"}

Erro:
{"non_field_errors":["Impossível fazer login com as credenciais fornecidas."]}

*************************************************************************************************

Instalação

Na pasta:
/var/www/security

- Criar virtualemv python 3:

pyvenv-3.5  env

- Clonar a aplicação:

git clone https://crleal@bitbucket.org/crleal/security_auth.git

- Usar o virtualenv criado:

source env/bin/activate

- cd security_auth/security_auth

- Instalando as dependencias do projeto na virtualenv:

pip install -r requirements.pip

- Criando a base de acordo com a configuração no setting.py:

python manage.py migrate

- criando um usuario admin:

python manage.py createsuperuser --username=admin --email=joe@example.com

como teste password: admin123


- Testando a aplicação sem configurar no servidor nginx:

python manage.py runserver   (servidor embutido para teste)

Starting development server at http://127.0.0.1:8000/

No caso do nosso servidor:

 http://198.50.250.135:8000/
