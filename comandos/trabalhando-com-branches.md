# Trabalhando com Branches

### **1 Criando uma nova branch**

```bash
git branch <nome da branch> // Apenas cria uma nova branch, não acessa

git checkout -b <nome da branch> // Criando e acessando uma nova branch
```

### **2 Retorna em um ponto específico e cria uma nova branch**

```bash
git checkout <insira o hash do commit> -b <nome da nova branch>
```

### **3 Renomeando as branches locais**

```bash
git branch -m <nome da branch> // Precisa estar na branch que deseja alterar

git branch -m <nome do antigo branch> <novo nome da branch> // Altera o nome de outra branch, enquanto está na master, por exemplo
```

### **4 Renomeando as branches remotas**

```bash
git branch -m <nome da branch> // Passo 1: primeiro alterar o nome da branch local e para isso é preciso estar na branch que deseja alterar

# Atenção: o comando abaixo exclui a branch remota. Tenha certeza de que possui a última versão da branch remota em seu repositório local para poder fazer o push dela logo em seguida.
git push origin :<nome do antigo branch> // Passo 2: substitua em <nome do antigo branch> pelo nome da sua branch antes de renomear

git push --set-upstream origin <novo nome da branch> // Passo 3: envia a branch renomeada para o repositório remoto

Pronto! Tanto a sua branch local quanto remota foram renomeadas.
```

### **5 Alterando de branch**

```bash
git checkout <nome da branch>
```

### **6 Visualizando todas as branches**

```bash
git branch // Existentes no repositório

git branch -a // Locais e remotos
```

### **7 Aplicando merge em branches**

```bash
git merge <nome da branch> // Precisa estar na branch de destino
```

### **8 Deletando uma branch local**

```bash
git branch -D <nome da branch>
```

### **9 Deletando uma branch remota**

```bash
git push origin :<nome da branch>
```