# Desafio Tech (Automação)
DesafioTech de Automação com Django e Django REST Framework.

***

## Preparação Inicial

Inicialmente, deve-se entrar no ambiente virtual, por meio do comando: <br/><br/>
`venv\Scripts\activate`<br/><br/>

E então, para iniciar o servidor, basta executá-lo com o manage.py:<br/><br/>
`python manage.py runserver`<br/><br/>

> Link do servidor: http://localhost:8000/

***

## Admin

> Link para o Admin: http://localhost:8000/admin/

![~ imagem do admin ~](https://github.com/AndreAndriotti/DesafioTech/blob/main/README_imagens/DesafioTech_Admin.png)

***

## Menu

> Link para o Menu: http://localhost:8000/Menu/

### _Lista de usuários_

![~ imagem da lista de usuários ~](https://github.com/AndreAndriotti/DesafioTech/blob/main/README_imagens/DesafioTech_ListaUsuarios.png)

### _Cadastrar usuários_

![~ imagem do cadastro ~](https://github.com/AndreAndriotti/DesafioTech/blob/main/README_imagens/DesafioTech_Cadastro.png)

### _Gerar senha aleatória (em progresso)_

Verificando se a senha foi deixada em branco:<br/><br/>
`if model.password == "":`<br/><br/>

Se foi, é gerada uma senha aleatória e atribuida ao usuário:<br/><br/>
`   password = User.objects.make_random_password()`<br/>
`   model.set_password(password)`<br/>
`   model.save()`<br/><br/>

### _Consultar usuários_

![~ imagem da consulta ~](https://github.com/AndreAndriotti/DesafioTech/blob/main/README_imagens/DesafioTech_Consulta.png)

### _Consultar/Exportar em diferentes formatos_

> Formatos permitidos:
> * API
> * XLSX
> * CSV
> * JSON

![~ imagem da consulta ~](https://github.com/AndreAndriotti/DesafioTech/blob/main/README_imagens/DesafioTech_FormatosArquivo.png)
