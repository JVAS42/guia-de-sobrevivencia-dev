<h1 align="center"> Guia de Comandos Git e GitHub (^._.^) </h1>

<h2 align="center"> Comandos Básicos </h2>

<h3 align="center"> Sincronizar Repositórios (Local e Remoto) </h3>

```bash
🔴🟡🟢
~ git init
~ git add . || ~ git add <NOME_ARQUIVO> # Adicionar todos os arquivos modificados OU Adicionar o arquivo modificado
~ git branch -M main
~ git remote add origin <HTTPS> || ~ git remote add origin <SSH>
~ git push -u origin main echo "Olá, Mundo!"
```

<h3 align="center"> Clonar um Repositório </h3>

```bash
🔴🟡🟢
~ git clone <HTTPS> || ~ git clone <SSH> 
```

<h3 align="center"> Realizar um commit </h3>

```bash
🔴🟡🟢
~ git status # (OPCIONAL) Mostrar histórico de modificações
~ git add . || ~ git add <NOME_ARQUIVO> # Adicionar todos os arquivos modificados OU Adicionar o arquivo modificado
~ git commit -m "<BREVE COMENTÁRIO SOBRE A MODIFICAÇÃO>"
~ git remote # (OPCIONAL) Verificar o repositório
~ git push origin main
```

<h3 align="center"> Baixar commit(s) </h3>

```bash
🔴🟡🟢
~ git pull origin main
~ git log # (OPCIONAL) Mostra o histórico de commmits
```

---

<h2 align="center"> Remover usuário do Git </h2>

<h3 align="center"> Windows </h3>

### Passo a passo para trocar de conta (HTTPS no Windows)
1. Apagar credenciais salvas
2. Abra o `Gerenciador de Credenciais` do Windows.
3. Vá em `Credenciais do Windows`.
4. Procure por entradas do tipo: `git:https://github.com` OU `git:https://gitlab.com`
5. No terminal, defina:

```bash
🔴🟡🟢
~ git config --global user.name "SeuNovoNome"
~ git config --global user.email "seuemail@novo.com"
```
6. Agora, quando você fizer `git pull` OU `git push` o Git vai pedir usuário e senha

---

<h2 align="center"> Comandos Avançados </h2>




