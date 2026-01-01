<h1 align="center"> Guia Inicial de Django com Ambiente Virtual 🐍 </h1>


<p align="center">
Este projeto tem como objetivo servir como guia prático para criação de um ambiente virtual em Python,
instalação do Django e configuração inicial de um projeto com aplicações.
</p>

<h2 align="center"> 🔹 Criando Ambiente Virtual </h2> 
<p align="center"> Cria ambientes isolados para diferentes projetos Python. </p> 
<h3 align="center"> Criar e Ativar Ambiente Virtual </h3>

```bash
🔴🟡🟢
~ python -m venv venv         # Cria um ambiente virtual chamado "venv"
~ venv\Scripts\activate       # Ativa o ambiente (Windows)
~ source venv/bin/activate    # Ativa o ambiente (Linux/Mac)
```

<h3 align="center"> Desativar Ambiente </h3>

```bash
🔴🟡🟢
~ deactivate                  # Desativa o ambiente virtual
```

<h2 align="center"> 🔹 Instalando o Django </h2> 

```bash
🔴🟡🟢
~ pip install django        # Instala o pacote desejado
```

<h3 align="center"> Iniciar um projeto </h3>

```bash
🔴🟡🟢
~ django-admin startproject <NOME_PASTA> . # Criar a pasta config
```

<h3 align="center"> Iniciar um server </h3>

```bash
🔴🟡🟢
~ python manage.py runserver # Iniciar server
```

```bash
➜ CTRL + C # Encerrar server
```

<h3 align="center"> Criar um aplicação </h3>

```bash
🔴🟡🟢
~ python manage.py startapp <NOME_PASTA> # Criar a pasta core, main ou web
```

```bash
Observação:
➜ OBS.: Para cada aplicacao criada, deve ser sinalida no settings.py em INSTALLED_APPS
models.py ➜ Modelo do banco de dados
views.py ➜ Logica das funcionalidades
```
