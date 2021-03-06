# INTRODUÇÃO AO GIT E GITHUB

## Comandos Básicos:

**cd (ls - linux):** change directions, navegar entre as pastas
   **cd ..:** retroceder
**TAB:** autocompleta a palavra 
**cls (clear ou ctrl L - linux)**: clear screen, limpar tela
**dir:** lista de diretórios para situar onde vc tá
**mkdir:** criar pasta 
**del:** deleta arquivos
**rmdir (rm - linux):** remove repositório
**echo:** escreve de volta a palavra /  escreve palavra num arquivo
**arrow key p cima:** histórico de comandos

## Git e Github

O Git é um sistema distribuído seguro

**Blobs:** guarda arquivos e metadados com sha1: tipo do objeto, tamanho, \0 e conteúdo
**Trees:** armazena blobs e metadados (com sha1), guarda o nome do arquivo e aponta para blobs ou outras trees
**Commits:** aponta para uma árvore, um parente, autor e mensagem também. possui timestamp e também possuem sha1 de todos os seus metadados

**Chave SSH:** conexão segura e encriptada entre 2 máquinas, sendo uma chave pública e outra privada
**Token de acesso pessoal:** substitui a senha do github, tem data de expiração. usa o protocolo https no github

**Tracked:** arquivos que o git tem ciência
  *unmodified:* não modificado
  *modified:* modificado (editado)
  *staged:* arquivos se preparando para poder fazer parte de um commit

**Untracked:** arquivos que o git não tem ciência

**Working Directory - Staging Area - Local Repository (composto por commits)** 

**Remote Repository**  

## Comandos:

**git init:** inicializa um repositório do git
**git add:** mover arquivos e conhecer primeiros comandos
  untracked => staged ou modified => staged
**git add *:** staged pra todos os arquivos
**git commit:** cria um commit
  staged => unmodified                                                                                                  **git commit -m “msg”:** envelopa arquivos numa msg e cria commit)
**git status:** diz se o arquivo está unmodified, modified ou staged
**git push:** empurra alterações para o repositório remoto
**git pull:** puxa alterações para o repositório local
**git clone:** clona o git de um repositório remoto p/ um local
**-a:** mostra arquivos ocultos

