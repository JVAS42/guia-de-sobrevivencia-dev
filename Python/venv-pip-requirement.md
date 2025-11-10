<h1 align="center"> Guia de Comandos Python: venv, pip e requirements.txt 🐍 </h1>

<h2 align="center"> 🔹 venv - Ambientes Virtuais </h2> 
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

<h2 align="center"> 🔹 pip - Gerenciador de Pacotes </h2> 
<p align="center"> Instalar, atualizar e remover pacotes Python. </p> 
<h3 align="center"> Instalar Pacotes </h3>

```bash
🔴🟡🟢
~ pip install <PACOTE>        # Instala o pacote desejado
~ pip install --upgrade pip   # Atualiza o pip
```

<h3 align="center"> Desinstalar Pacotes </h3>

```bash
🔴🟡🟢
~ pip uninstall <PACOTE>      # Remove o pacote
```

<h3 align="center"> Listar Pacotes Instalados </h3>

```bash
🔴🟡🟢
~ pip freeze                  # Mostra todos os pacotes instalados
```

<h2 align="center"> 🔹 requirements.txt - Gerenciamento de Dependências </h2> 
<p align="center"> Cria e instala listas de pacotes para replicar o ambiente. </p> 
<h3 align="center"> Criar requirements.txt </h3>

```bash
🔴🟡🟢
~ pip freeze > requirements.txt    # Cria o arquivo com todos os pacotes instalados
```

<h3 align="center"> Instalar a partir do requirements.txt </h3>

```bash
🔴🟡🟢
~ pip install -r requirements.txt  # Instala todos os pacotes listados no arquivo
```

<h2 align="center"> 💡 Dicas Extras </h2>
```bash
🔴🟡🟢
~ python --version            # Verifica a versão do Python
~ pip --version               # Verifica a versão do pip
~ where python                # Mostra o caminho do Python (Windows)
~ which python                # Mostra o caminho do Python (Linux/Mac)
```
