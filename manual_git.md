
# 📘 Manual de Consulta – Git & GitHub / Git & GitHub Reference Manual

> Manual prático de comandos Git para uso diário.  
> Practical manual of Git commands for daily use.  
> Repositório oficial / Official repository: [comandosgit](https://github.com/GHF-BR/comandosgit.git)

---

## 🔹 1. Configuração inicial / Initial setup

```bash
# Nome do usuário / User name
git config --global user.name "Seu Nome / Your Name"

# E-mail do usuário / User email
git config --global user.email "seuemail@exemplo.com"

# Ver configurações / Check settings
git config --list
```

---

## 🔹 2. Criando e clonando repositórios / Creating and cloning repositories

```bash
# Criar um repositório local / Create a local repository
git init

# Clonar um repositório remoto / Clone a remote repository
git clone https://github.com/usuario/repositorio.git
```

---

## 🔹 3. Ciclo básico do Git / Basic Git workflow

```bash
# Verificar status / Check status
git status

# Adicionar arquivo específico / Add a specific file
git add nome_do_arquivo

# Adicionar todos os arquivos / Add all files
git add .

# Criar commit / Create commit
git commit -m "mensagem descritiva / descriptive message"

# Histórico de commits / Commit history
git log
```

---

## 🔹 4. Enviar e atualizar do GitHub / Push and pull from GitHub

```bash
# Enviar commits para a branch principal / Push commits to main branch
git push origin main

# Baixar atualizações do remoto / Pull updates from remote
git pull origin main
```

---

## 🔹 5. Branches (ramificações)

```bash
# Criar nova branch / Create new branch
git branch nome-branch

# Listar branches / List branches
git branch

# Trocar de branch / Switch branch
git checkout nome-branch

# Criar e trocar ao mesmo tempo / Create and switch
git checkout -b nome-branch

# Mesclar branch com a principal / Merge branch into main
git checkout main
git merge nome-branch
```

---

## 🔹 6. Gitignore

No arquivo **.gitignore**, defina arquivos e pastas a ignorar.  
In the **.gitignore** file, define files and folders to ignore.

Exemplo / Example:
```
*.log
*.tmp
node_modules/
venv/
```

Criar / Create:
```bash
touch .gitignore
```

---

## 🔹 7. Desfazendo alterações / Undoing changes

```bash
# Remover arquivo do stage / Unstage file
git reset nome_arquivo

# Descartar mudanças em arquivo / Discard changes in file
git checkout -- nome_arquivo

# Resetar tudo para último commit / Reset everything to last commit
git reset --hard HEAD
```

---

## 🔹 8. Repositório remoto / Remote repository

```bash
# Adicionar repositório remoto / Add remote repository
git remote add origin https://github.com/usuario/repositorio.git

# Verificar remotos configurados / Check configured remotes
git remote -v
```

---

## 🔹 9. Comandos úteis / Useful commands

```bash
# Ver diferenças nos arquivos / Show file differences
git diff

# Histórico resumido com gráfico / Summarized log with graph
git log --oneline --graph --all

# Clonar já na branch 'main' / Clone directly into 'main' branch
git clone -b main https://github.com/usuario/repositorio.git
```

---

## 🔹 10. Fluxo de trabalho recomendado / Recommended workflow

1. **Atualizar antes de começar / Update before starting**  
   ```bash
   git pull origin main
   ```
2. **Fazer mudanças / Make changes**  
3. **Adicionar arquivos / Add files**  
   ```bash
   git add .
   ```
4. **Criar commit / Create commit**  
   ```bash
   git commit -m "Descrição clara / Clear description"
   ```
5. **Enviar ao GitHub / Push to GitHub**  
   ```bash
   git push origin main
   ```

---

## 🔹 11. Resumo prático (cola rápida) / Quick reference (cheat sheet)

```bash
# Inicialização / Init
git init
git clone <url>

# Ciclo / Workflow
git status
git add .
git commit -m "mensagem / message"
git push origin main
git pull origin main

# Branches
git checkout -b nova / new
git checkout main
git merge nova / new

# Desfazer / Undo
git reset arquivo / file
git checkout -- arquivo / file
git reset --hard HEAD
```

---

## 🔹 12. Recursos adicionais / Additional resources

- 📖 [Documentação Git / Git Docs](https://git-scm.com/doc)  
- 📘 [Guia GitHub / GitHub Guide](https://docs.github.com/)  
- 🔧 [Gerar .gitignore automático / Generate .gitignore](https://www.toptal.com/developers/gitignore)  

---

✍️ **Dica / Tip:** Sempre escreva mensagens de commit **claras e objetivas / clear and objective**.  
🔄 **Boa prática / Best practice:** Faça `git pull` antes de começar a trabalhar / Always `git pull` before starting work.  
