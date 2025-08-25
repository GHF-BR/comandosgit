
# 📘 Manual de Consulta – Git & GitHub

> Manual prático de comandos Git para uso diário.  
> Repositório oficial: [comandosgit](https://github.com/GHF-BR/comandosgit.git)

---

## 🔹 1. Configuração inicial

```bash
# Nome do usuário
git config --global user.name "Seu Nome"

# E-mail do usuário
git config --global user.email "seuemail@exemplo.com"

# Ver configurações
git config --list
```

---

## 🔹 2. Criando e clonando repositórios

```bash
# Criar um repositório local
git init

# Clonar um repositório remoto
git clone https://github.com/usuario/repositorio.git
```

---

## 🔹 3. Ciclo básico do Git

```bash
# Verificar status
git status

# Adicionar arquivo específico
git add nome_do_arquivo

# Adicionar todos os arquivos
git add .

# Criar commit
git commit -m "mensagem descritiva"

# Histórico de commits
git log
```

---

## 🔹 4. Enviar e atualizar do GitHub

```bash
# Enviar commits para a branch principal (main ou master)
git push origin main

# Baixar atualizações do remoto
git pull origin main
```

---

## 🔹 5. Branches (ramificações)

```bash
# Criar nova branch
git branch nome-branch

# Listar branches
git branch

# Trocar de branch
git checkout nome-branch

# Criar e trocar ao mesmo tempo
git checkout -b nome-branch

# Mesclar branch com a principal
git checkout main
git merge nome-branch
```

---

## 🔹 6. Gitignore

No arquivo **.gitignore**, defina arquivos e pastas a ignorar.

Exemplo:
```
*.log
*.tmp
node_modules/
venv/
```

Criar:
```bash
touch .gitignore
```

---

## 🔹 7. Desfazendo alterações

```bash
# Remover arquivo do stage
git reset nome_arquivo

# Descartar mudanças em arquivo
git checkout -- nome_arquivo

# Resetar tudo para último commit
git reset --hard HEAD
```

---

## 🔹 8. Repositório remoto

```bash
# Adicionar repositório remoto
git remote add origin https://github.com/usuario/repositorio.git

# Verificar remotos configurados
git remote -v
```

---

## 🔹 9. Comandos úteis

```bash
# Ver diferenças nos arquivos
git diff

# Histórico resumido com gráfico
git log --oneline --graph --all

# Clonar já na branch 'main'
git clone -b main https://github.com/usuario/repositorio.git
```

---

## 🔹 10. Fluxo de trabalho recomendado

1. **Atualizar antes de começar**  
   ```bash
   git pull origin main
   ```
2. **Fazer mudanças**  
3. **Adicionar arquivos**  
   ```bash
   git add .
   ```
4. **Criar commit**  
   ```bash
   git commit -m "Descrição clara"
   ```
5. **Enviar ao GitHub**  
   ```bash
   git push origin main
   ```

---

## 🔹 11. Resumo prático (cola rápida)

```bash
# Inicialização
git init
git clone <url>

# Ciclo
git status
git add .
git commit -m "mensagem"
git push origin main
git pull origin main

# Branches
git checkout -b nova
git checkout main
git merge nova

# Desfazer
git reset arquivo
git checkout -- arquivo
git reset --hard HEAD
```

---

## 🔹 12. Recursos adicionais

- 📖 [Documentação Git](https://git-scm.com/doc)  
- 📘 [Guia GitHub](https://docs.github.com/)  
- 🔧 [Gerar .gitignore automático](https://www.toptal.com/developers/gitignore)  

---

✍️ **Dica:** Sempre escreva mensagens de commit **claras e objetivas**.  
🔄 **Boa prática:** Faça `git pull` antes de começar a trabalhar.  
