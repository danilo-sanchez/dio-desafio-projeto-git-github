# Git e Github

#### Como o Git Funciona

SHA1 - SHA significa Secure Hash Algorithm (Algoritmo de Hash Seguro)
Conjunto de funcoes hash criptograficas projetadas pela NSA (Agencia de Segurança Nacional dos EUA)
A encriptacao gera conjunto de caracteres identificador de 40 digitos.

#### Objetos Internos do Git

- Blobs (bolhas - objeto git) - contem metadados do git (tipo do objeto, tamanho da string, tamanho do arquivo, etc)
blob 9\0conteudo

- Trees (Arvores) - armazenam blobs - contem metadados (tipo do blob, sha1 e nome do arquivo)

- Commits (aponta para Arvore, parente (ultimo commit), autor, mensage, timestamp)

## Comandos Git

#### Iniciar o GIT no diretorio atual
```
git init
```

#### Iniciar o versionamento (move do "working directory" para "staging area")
```
git add nomedoarquivo
git add *
git add .
```

#### Criar um commit (move da staging area para local repository)
```
git commit -m "mensagem descrevendo as alteracoes"
```

#### Inserindo E-mail e Nome de Usuario no Git
```
git config --global user.email "seuemail"
git config --global user.name "seunomedeusuario"
```

#### Excluindo E-mail e Nome de Usuario no Git
```
git config --global --unset user.email
git config --global --unset user.name
```

#### Verificar o status dos arquivos
```
git status
```

#### Configurando o repositorio remoto:
```
git remote add origin https://github.com/seunomedeusuario/repositorio.git
```

#### Enviando o codigo para o servidor remoto:
```
git push origin main
```

#### Puxando o codigo do servidor remoto para o repositorio local:
```
git pull origin master
```

#### Clonando Repositorios do Github:
```
git clone https://github.com/nomedeusuario/repositorio.git
```