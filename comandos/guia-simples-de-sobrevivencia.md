# Guia Simples de Sobrevivência

### **1 Configurações iniciais do Git**

**Baixando e instalando o Git**

[`https://git-scm.com/`](https://git-scm.com/)

**Exibe a versão do Git instalado**

`git --version`

**Configura nome de usuário**

`git config --global user.name <seu nome aqui>`

**Configura email de usuário**

`git config --global user.email <seu email aqui>`

### **2 Inicializando um repositório**

**Inicializa o versionamento no respectivo diretório**

`git init`

### **3 Comandos básicos**

**Verifica o status do repositório**

`git status`

**Adiciona todos os arquivos para serem commitados**

`git add .`

**Commitando arquivos**

`git commit -m <insira um comentário significativo>"`

> [6 Boas Práticas de Commit](https://blog.locaweb.com.br/temas/codigo-aberto/6-boas-praticas-de-git/)
> 

**Visualizando relatório de commits**

```bash
git log // Exibe todos os commits

git log --oneline // Exibe todos os commits em um única linha de forma reduzida

git log -p // Exibe todas as alterações dos commits
```

> Existe uma infinidade de formatos que podemos usar como filtros para mostrar nosso histórico, e em [git log cheatsheet](http://devhints.io/git-log) há vários delas.
> 

### 4 Removendo arquivo/diretório

**Removendo arquivo**

`git rm meu_arquivo.txt`

**Removendo diretório**

`git rm -r diretorio`

### 5 Ignorando arquivo

> Existe um **arquivo especial do Git**, chamado `.gitignore`, e todas as linhas que estiverem nele serão lidos e ignorados pelo Git. Se temos um arquivo denominado `ide-config` que queremos que seja ignorado, por exemplo, basta o incluirmos em `.gitignore`, digitando `ide-config` simplesmente. Da mesma forma, se tivéssemos uma pasta `ide`, incluiríamos `ide/`, em uma nova linha.
> 

### 6 Criando um repositório remoto no GitHub

**Adicionando um repositório remoto**

`git remote add origin https://github.com/*USERNAME*/*REPOSITORY*.git`

**Enviando as modificações para o repositório remoto**

`git push origin <nome da branch>`

### 7 **Trabalhando com branches (trabalhando em equipe)**

**Criando e acessando para uma nova branch**

`git checkout -b <nome da branch>`

**Visualizando todas as branches existentes no repositório**

`git branch`

**Alterando de branches**

`git checkout <nome da branch>`

**Aplicando merge em branches**

`git merge <nome da branch> // Precisa estar na branch de destino`

**Baixando alterações do GitHub para a sua máquina (se o repositório for de sua autoria)**

`git pull origin <nome da branch>`

**Deletando uma branch local**

`git branch -D <nome da branch>`

**Deletando uma branch remota**

`git push origin :<nome da branch>`

### 8 Clonando um repositório para a sua máquina

**Copiando o link no GitHub**

> Copie o link HTTPS que aparecerá ao clicar no botão `Code`
> 

**Puxando o projeto para máquina no GitBash**

`git clone + o link HTTPS copiado acima`

### **9 Baixando as alterações do GitHub para a sua máquina**
 (se o repositório for de sua autoria)

`git pull origin <branch>`