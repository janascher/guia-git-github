# Trabalhando com Commits

### **1 Commitando**

`git commit -m "insera um comentário significativo"`

### **2 Desfazendo alterações antes de adicioná-las (antes de fazer `git add`)**

`git checkout`

### **3 Desfazendo alterações depois de adicioná-las (depois de fazer `git add`)**

`git reset HEAD "nome do arquivo"`

### **4 Desfazendo um commit**

`git revert "insira o hash do commit"`

> Para encontrar o hash do commit, é preciso rodar no terminal o `git log` para visualizar o histórico de commits.
> O hash é o código composto de letras e números que aparece em `commit: XXXXXXXXX`.