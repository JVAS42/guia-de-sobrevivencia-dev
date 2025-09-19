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

<h3 align="center"> Criando e atualizando Branchs </h3>

```bash
🔴🟡🟢
~ git branch <NOME_BRANCH> # Cria a branch
~ git chekout <NOME_BRANCH> # Alterar para a branch || ~ git switch -c <NOME_BRANCH> # Cria e altera para a branch

~ git push origin <NOME_BRANCH> # Subir alterações dessa branch

~ git release main # Atualiza a branch com versão mais atualizada da `main`
```

<h3 align="center"> Excluir uma branch </h3>

```bash
🔴🟡🟢
~ git branch -d <NOME_BRANCH> # Excluir uma branch
```

<h3 align="center"> Unir Branchs </h3>

```bash
🔴🟡🟢
~ git merge <NOME_BRANCH> # Unir a nova branch com a main
```

<h3 align="center"> Histórico de commits </h3>

<p align="center"> LOG </p>

```bash
🔴🟡🟢
~ git log --oneline #Mostra todos os commits
~ git log --p # Mostra commit com mais detalhes
~ git log --graph # Mostra a linha do tempo dos commits
~ git log --format "..." # Mostra commits detalhados
~ git log --help # Ajuda sobre os comandos
```

- SAIR DO LOG: tecla `Q`

<p align="center"> DIFF </p>

```bash
🔴🟡🟢
~ git log --oneline
~ git log --p
~ git log --graph
~ git log --format "..."
~ git log --help 
```

<h3 align="center"> Versões </h3>

<p align="center"> STASH </p>

```bash
🔴🟡🟢
~ git stash # Guarda estado
~ git stash pod # Pega estado
~ git stash list # Lista estados
~ git stash clear # Limpa estado
~ git stash push -m "<MENSAGEM>" # Lista commits
```

<p align="center"> RESTORE </p>

```bash
🔴🟡🟢
~ git restore . || ~ git restore <NOME_ARQUIVO> # Restaurar código
```

<h3 align="center"> Gerando entregas </h3>

```bash
🔴🟡🟢
~ git tag -a <NOME_VERSAO> -m "<COMMIT>" # Criar um tag da versão

~ git tag -d <NOME_VERSAO> # Remover a tag da versão

~ git push origin --tags || ~ git push origin --tags # Subir uma tag
```

