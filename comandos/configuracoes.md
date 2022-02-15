# Configurações

Observação:
No Git Bash os comandos são iniciados com $ que são inseridos automaticamente pela ferramenta. Em razão disso, ocultei o $ nos exemplos abaixo.

### **1 Locomovendo entre pastas**

```bash
cd <nome-da-pasta>

cd .. // Retorna 1 pasta

cd - // Retorna para pasta que estava anteiormente

```

### **2 Abrindo o VS Code**

```bash
code
```

### **3 Abrindo o projeto no VS Code**

```bash
code .
```

### **4 Abrindo o Windows Explorer**

```bash
explorer
```

### **5 Abrindo o Windows Explorer na pasta que estamos atualmente**

```bash
explorer .
```

### **6 Configura nome de usuário**

```bash
git config --global user.name seu nome aqui
```

### **7 Configura email de usuário**

```bash
git config --global user.email seu email aqui
```

### **8 Visualiza configurações de usuário**

```bash
git config -l
# ou
git config --list
```

### **9 Visualizando a versão do Git Bash**

```bash
git --version
```