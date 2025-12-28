---
title: "O Passo a Passo: Construindo a Documentação"
author: Ana Claudia
date: 2025-12-01
wordCount: false
---

Este guia descreve as etapas exatas para configurar o ambiente e colocar o site no ar, garantindo que a estrutura de pastas e ferramentas funcionem em harmonia.

## 1. Configurando o GitHub
O repositório é o alicerce do projeto.
* **Criação**: Crie um repositório público no GitHub.
* **Clone**: Baixe o projeto para sua máquina local:
    ```bash
    git clone [https://github.com/SEU_USUARIO/seu-repositorio.git](https://github.com/SEU_USUARIO/seu-repositorio.git)
    ```

## 2. Configurando o VS Code
O editor deve estar preparado para lidar com Markdown e o terminal.
* **Abertura**: Abra a pasta raiz (onde está o arquivo `hugo.toml`).
* **Terminal**: Utilize o terminal integrado (`Ctrl + '`) para garantir que você está executando comandos no contexto correto do projeto.
* **Extensões**: Instale "Markdown All in One" para visualizar o progresso da escrita em tempo real.

## 3. Estruturando o Conteúdo (Hugo)
Nesta etapa, definimos a arquitetura de pastas dentro de `content/posts`:
* Organize os arquivos com numeração (ex: `0-`, `1-`, `2-`) para garantir que o Hugo siga a ordem lógica na navegação.
* Mantenha os arquivos `.md` com nomes claros e sem espaços.

## 4. Rodando o Servidor Local
Para visualizar as alterações antes de publicar:
1. Certifique-se de que o terminal está na **raiz do projeto** (onde o `hugo.toml` reside).
2. Execute o comando:
   ```bash
   hugo server -D