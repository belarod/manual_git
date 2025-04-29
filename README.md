# Manual Git

## Pré-requisitos
- Git instalado ([Download](https://git-scm.com/))

---

## Configuração Inicial

### 1. Iniciar repositório local
```bash
git init
```
### 2. Renomear branch principal (boas práticas)
```bash
git branch -m master main
```
### 3. Conectar ao repositório remoto
```bash
git remote add origin <URL>
# Exemplo:
git remote add origin https://github.com/ermidapablo/engsw-2025-1.git
```
---

## Fluxo Básico de Trabalho

### Preparar mudanças
```bash
git add <arquivo>       # Arquivo específico
git add .               # Todos os arquivos alterados
```
### Verificar status
```bash
git status
```
### Registrar alterações
```bash
git commit -m "mensagem"   # Forma rápida
git commit                 # Abre editor de texto (CTRL+X → Y → ENTER no Nano)
```
### Enviar para o remoto
```bash
git push origin <branch>   # Ex: git push origin main
```
### Atualizar do remoto
```bash
git pull origin <branch>   # Ex: git pull origin main
```
---

## Gerenciamento de Branches

### Sincronizar branches remotas
```bash
git fetch
```
### Listar branches
```bash
git branch      # Locais
git branch -r   # Remotas
```
### Trocar de branch
```bash
git checkout <branch>  #Ex: git checkout cadastro-do-usuario
```

---

## Boas Práticas para Projetos Colaborativos

### 1. Sempre comece com repositório limpo:
```bash
git init                        #Ex: em uma pasta vazia...
git remote add origin <URL>
git pull origin main
```
### 2. Trabalhe em sua própria branch:
```bash
git checkout <branch>   # Muda para respectiva branch
```
## Material de apoio

Acesse o [Git Cheat Sheet (PDF)](https://education.github.com/git-cheat-sheet-education.pdf) 🔗.

### Para configurar o Nano como editor de texto:
```bash
git config --global core.editor "nano"
```
