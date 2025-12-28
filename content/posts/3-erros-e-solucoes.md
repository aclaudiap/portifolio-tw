---
title: "Troubleshooting"
date: 2025-12-28
author: Ana Claudia
wordCount: false
---
# Erros Conhecidos e Soluções (Troubleshooting)

Nesta seção, registro os principais desafios técnicos encontrados durante a configuração do ambiente e como foram resolvidos.

## 1. Comando não reconhecido no Terminal (Node/Hugo/Git)

**Problema:** Ao tentar rodar comandos como `hugo server`, `npm install` ou `git`, o terminal retorna o erro:
> "O termo 'comando' não é reconhecido como nome de cmdlet, função, arquivo de script ou programa operável."

**Causa:** Isso ocorre geralmente após uma nova instalação ou atualização. O executável da ferramenta foi baixado, mas o sistema operacional não sabe onde ele está localizado porque o caminho (path) não foi adicionado às **Variáveis de Ambiente**.

**Solução (Passo a Passo no Windows):**
1. Pressione a tecla `Win` e digite **"Editar as variáveis de ambiente do sistema"**.
2. Na janela que abrir, clique no botão **Variáveis de Ambiente** (canto inferior direito).
3. Na seção **Variáveis do sistema**, localize a variável chamada `Path` e clique em **Editar**.
4. Verifique se o caminho da pasta `bin` da ferramenta (ex: `C:\Hugo\bin` ou `C:\Program Files\nodejs\`) está na lista.
5. Caso não esteja, clique em **Novo** e cole o caminho completo da pasta onde está o arquivo `.exe`.
6. Clique em **OK** em todas as janelas.
7. **Importante:** Feche e abra novamente o VS Code ou o terminal para que as alterações entrem em vigor.

---

## 2. Erro de Permissão de Script (PowerShell)

**Problema:** Ao tentar executar scripts de automação, o Windows bloqueia a execução por política de segurança.

**Solução:** Abra o PowerShell como Administrador e execute:
```powershell
Set-ExecutionPolicy -ExecutionPolicy RemoteSigned -Scope CurrentUser