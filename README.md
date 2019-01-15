# Website whith Django

## Instalação

Crie e ative um ambiente virtual e realize a instalação do requisito disponível no arquivo *requirements.txt*.
```
pip install -r requirements.txt
```

Execute o servidor com o comando:
```
python manage.py runserver
```
Acese a pagina [localhost:8000](http://localhost:8000/)

## Banco de Dados

O bando de dados disponível é *db.sqlite3*, caso não seja localizado, execute o comando para criação do bando de dados:
```
python manage.py migrate
```

Adicione usuário administrador para o banco de dados com o comando:
```
python manage.py createsuperuser
```
Adicione itens às tabelas acessando a página [localhost:8000/admin](http://localhost:8000/admin/) com o usuário e senha definidos anteriormente.

## Aplicando mudanças CSS

Quando alterações no arquivo css não estiverem sendo aplicadas, realizar:
```
python manage.py collectstatic
```
