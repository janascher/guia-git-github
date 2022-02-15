# Trabalhando com Commits

### **1 Commitando**

```bash
git commit -m "insera um comentário significativo"
```

### **2 Desfazendo alterações antes de adicioná-las (antes de fazer `git add`)**

```bash
git checkout -- <nome do arquivo>
```

### **3 Desfazendo alterações depois de adicioná-las (depois de fazer `git add`)**

```bash
git reset HEAD <nome do arquivo>
```

### **4 Desfazendo um commit**

```bash
git revert <insira o hash do commit>
```

> Para encontrar o hash do commit, é preciso rodar no terminal o `git log` para visualizar o histórico de commits.
> O hash é o código composto de letras e números que aparece em `commit: XXXXXXXXX`.

### **5 Guardando alterações temporariamente e que ainda não foram commitadas para o stash**

```bash
git stash
```

### **6 Visualizando os itens guardados no stash**

```bash
git stash list
```

### **7 Trazendo os itens guardados no stash para o diretório de trabalho**
(porém elas continuarão na stash, portanto será preciso removê-las depois)

```bash
git stash apply <número do stash>
```

> Para encontrar o número do stash, é preciso rodar no terminal o `git stash list` para visualizar o histórico do stash.
> O número do stash fica entre {} (chaves), por exemplo `stash@{0}: WIP on master`.

### **8 Removendo as alterações do stash**

```bash
git stash drop
```

### **9 Trazendo os itens guardados no stash para o diretório de trabalho + Removendo as alterações do stash**
(fazer ambas as ações ao mesmo tempo)

```bash
git stash pop
```

> Ao ser executado, realiza o merge com as alterações e aplica aquelas que estavam salvas lá.

### **10 Removendo todos os stash**

```bash
git stash clear
```

### **11 Visualizando relatórios de commits**

```bash
git log // Exibe todos os commits

git log --oneline // Exibe todos os commits em um única linha de forma reduzida

git log -p // Exibe todas as alterações dos commits
```

### **12 Visualizando as diferenças de commits**

```bash
git diff // Mostra o que foi alterado e que ainda não foi adicionado para commit

git diff {hash do commit de merge com lista}...{hash do último commit realizado} // Os três pontinhos (...) significam "até"
```