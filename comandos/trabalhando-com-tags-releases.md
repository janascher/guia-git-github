# Trabalhando com Tags e Releases

### **1 Criando uma tag**

```bash
git tag -a "insira a versão" // Apenas criando uma tag

git tag -a "insira a versão" -m "insira um comentário significativo" // Criando tag e incluindo um commit
```
Exemplo:
```bash
git tag -a v0.1.0

git tag -a v0.1.0 -m "Lança a primeira versão (BETA) da aplicação de cursos" // Criando tag e incluindo um commit
```
### **2 Visualizando histórico de tags criadas**

```bash
git tag
```

### **3 Enviando a tag criada para o servidor (GitHub)**

```bash
git push master // Primeiro passo

git push v0.1.0 // Segundo passo

# Deste modo criamos 1 release, que é a versão pronta para ser lançada ou baixada por qualquer pessoa que queira utilizar.
```