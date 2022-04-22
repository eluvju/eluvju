```python
pip install pipreqs

pipreqs /path/to/project
```

python -m venv venv
.\\venv\\Scripts\\Activate

pip install -r requirements.txt

django-admin startproject helloproject .

python manage.py runserver

python manage.py startapp `nomedoprojecto`

OBS: Verificar SEMPRE se a pasta do projecto não esta dentro de outra pasta por ENGANO

## Fase 2, URLS

- 1: Alterar Project/urls
	- `DE` from django.urls import path 
	- `PARA` from django.urls import path, include  

- 2: Criar Arquivo urls.py na pasta APP

Layout Basico
![[Pasted image 20220419154620.png]]

- 3: `views.py` Criar os DEF de pathing das paginas e importar lib `HTTP RESPONSE`


## Fase 3, HTML -  Pasta Templates no APP

- 1: Crie uma pasta com o nome `TEMPLATES` e dentro dela uma pasta com o nome do Aplicativo Ex: `VPOK`.

- 2: Dentro da pasta você cria o arquivo `HTML` com o comando `!`

---

PRIMEIROS PASSOS PAGINA HTML

- 1: Adicionar as Sheets and Libraries que vc vai usar inicialmente no site.

### Libraries CSS

https://cdnjs.com/libraries/font-awesome

- 2: Criar "Containers" que separam a pagina em Blocos

OBS: 1.0rem = 10 pixels, 1.6rem = 16 pixels...

- 3: Criar pastas `PAGES` e `PARTIALS` em templates/projeto
	-  `PAGES` = São as paginas Ex: Home
	- `PARTIALS` = Partes fixas do site Ex: Header
- 4: Criar o arquivo head.html na pasta partials e mover sua HEADER para lá
	- Utilizar comando `INCLUDE` para migrar a header para a home

![[Pasted image 20220420031816.png]]

OBS: qualquer comando seja ele INCLUDE, IF OU FOR são utilizados `{%  %}`








---

# Boas Maneiras

Arquivos, Codigos entre outras coisas sempre em `Ingles`

Usar `Run and Debugg` Para Automatizar Funções configurando ele pelo "Launch.json"



---

Init.py 
- Serve para indicar para o python que a esta projeto é um pacote do python
- Serve para export

Asgp.py | wsgi.py
- Web Server interface
- Serve para fazer a ligação com web Server

settings.py

-Configurações do djangou

urls.py

- Porta de entrada da Interface

---

Resposta HTTP 

Como fazer um pathing até um diretório diferente utilizando (Request) e o servidor retorna.

![[Pasted image 20220417033933.png]]

Codigo de Status de Resposta: 

https://developer.mozilla.org/pt-BR/docs/Web/HTTP/Status

![[Pasted image 20220418165304.png]]

---


---

# Correção de Erros

Emmet abreviation = Solução

![[Pasted image 20220419150229.png]]

TemplateDoesNotExist At /

Adicionar o App no arquivo Settings.py 

![[Pasted image 20220419150832.png]]

Adicionar Pastas adicionais ao APP (Base Templates)

![[Pasted image 20220419152150.png]]

Corrigir Erros de Duplicação de Arquivos (Name Space)

![[Pasted image 20220419152331.png]]

`{{}}` Exibe uma variavel no arquivo HTML


---

# Comandos de Django para HTML

### Incluir uma pagina em outra

**Comando Include**: 
![[Pasted image 20220420032114.png]]

