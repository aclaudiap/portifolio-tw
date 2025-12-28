---
title: "Ferramentas e Acessos"
date: 2025-12-26
author: Ana Claudia
wordCount: false
---

Para construir e manter esta documentação, foi necessário configurar um ambiente de desenvolvimento local. Abaixo estão as ferramentas utilizadas e os acessos configurados.

## 🛠️ Ferramentas de Software

### 1. Hugo (Static Site Generator)
O motor principal deste site. Foi escolhido pela sua velocidade e simplicidade.
* **Versão:** Extended (recomendada para temas como o FixIt).
* **Configuração Crítica:** A pasta `bin` do Hugo deve estar no **Path** das Variáveis de Ambiente do Windows para que o comando `hugo server` funcione em qualquer diretório.

### 2. Git (Controle de Versão)
Essencial para gerir as alterações e fazer o deploy para o GitHub.
* **Comando de verificação:** `git --version`
* **Uso:** Sincronização entre a máquina local e o repositório remoto.

### 3. VS Code (Editor de Código)
Onde toda a escrita em Markdown acontece.
* **Extensões Utilizadas:**
    * **Markdown All in One:** Para pré-visualização e atalhos de formatação.
    * **FixIt Theme Support:** (Opcional) Para facilitar a edição do `hugo.toml`.

### 4. Node.js & NPM
Necessários para gerir dependências de alguns temas e ferramentas de automação.
* **Verificação:** `node -v` e `npm -v`

---

## 🔑 Acessos e Plataformas

### GitHub & GitHub Pages
* **Repositório:** `aclaudiap/portifolio-tw`
* **Hospedagem:** O site é servido através do domínio `github.io` de forma gratuita.
* **Autenticação:** Configurada via Git Bash (SSH ou Credential Manager do Windows).

---

## 💡 Checklist de Instalação (Pós-Reinstalação)
Sempre que o ambiente for formatado ou as ferramentas reinstaladas, verifica:
1. [ ] O executável do Hugo está na pasta `C:\Hugo\bin` (ou similar)?
2. [ ] O **Path** nas Variáveis de Sistema foi atualizado?
3. [ ] O terminal do VS Code reconhece o comando `hugo version`?

---
*Dica: Se algum comando acima falhar, consulta a nossa página de [Erros e Soluções](./3-erros-e-solucoes.md).*