# 🛠️ Guia de Instalação — Claude Code + Notion MCP

Este guia é para quem quer usar a versão com IA da skill. Se prefere montar manualmente no Notion, veja o [guia de montagem](../notion/guia-de-montagem.md).

---

## Pré-requisitos

| Requisito | Gratuito? | Link |
|-----------|-----------|------|
| Node.js 18+ | ✅ Sim | [nodejs.org](https://nodejs.org) |
| Claude Code CLI | ✅ Plano gratuito disponível | [claude.ai/code](https://claude.ai/code) |
| Conta no Notion | ✅ Plano gratuito funciona | [notion.so](https://notion.so) |
| Notion MCP conectado | ✅ Incluído no Claude Code | — |

---

## Passo 1 — Instalar o Claude Code

```bash
npm install -g @anthropic-ai/claude-code
```

Verifique a instalação:

```bash
claude --version
```

Faça login com sua conta Anthropic:

```bash
claude
```

Na primeira execução, ele vai pedir autenticação via browser.

---

## Passo 2 — Conectar o Notion MCP

O Notion MCP é a integração que permite ao Claude ler e escrever no seu Notion.

1. Abra o Claude Code
2. Digite `/mcp` para acessar as configurações de MCP
3. Procure por **Notion** e clique em **Connect**
4. Faça login com sua conta Notion quando solicitado
5. Autorize o acesso ao workspace onde você quer criar a estrutura

> Se não aparecer a opção Notion em `/mcp`, verifique se está usando Claude Code versão mais recente (`npm update -g @anthropic-ai/claude-code`).

---

## Passo 3 — Copiar a skill

Crie a pasta da skill:

```bash
mkdir -p ~/.claude/skills/notion-eisenhower
```

Copie o arquivo [SKILL.md](../skill/SKILL.md) para essa pasta:

**Opção A — via curl:**
```bash
curl -o ~/.claude/skills/notion-eisenhower/SKILL.md \
  https://raw.githubusercontent.com/anialquimiadigital-creator/eisenhower-ai-daily/main/skill/SKILL.md
```

**Opção B — manualmente:**
1. Abra o arquivo [skill/SKILL.md](../skill/SKILL.md) neste repositório
2. Copie todo o conteúdo
3. Cole em `~/.claude/skills/notion-eisenhower/SKILL.md`

---

## Passo 4 — Testar a instalação

Abra o Claude Code em qualquer pasta:

```bash
claude
```

Digite:
```
criar minha estrutura no Notion
```

A skill deve ser ativada e fazer as perguntas iniciais (nome, áreas de trabalho, gestor).

Se não ativar, verifique se o arquivo está no caminho correto:

```bash
ls ~/.claude/skills/notion-eisenhower/
# deve mostrar: SKILL.md
```

---

## Passo 5 — Uso diário

A skill é ativada automaticamente quando você usa frases como:

```
bom dia
captura: reunião com cliente amanhã, ideia de novo produto, ligar pro contador
fechando o dia
relatório semanal
```

Não precisa abrir um projeto específico. Funciona de qualquer diretório.

---

## Resolução de problemas

**A skill não aparece / não é ativada:**
- Confirme que o arquivo está em `~/.claude/skills/notion-eisenhower/SKILL.md`
- Reinicie o Claude Code
- Verifique se o nome do arquivo é exatamente `SKILL.md` (maiúsculo)

**Erro de permissão do Notion:**
- Acesse [notion.so/my-integrations](https://notion.so/my-integrations)
- Confirme que a integração do Claude está conectada ao workspace correto
- Re-autorize se necessário

**"notion-search não encontrou nada":**
- O Notion MCP só acessa páginas que foram compartilhadas com a integração
- No Notion, abra cada página raiz → Share → adicione a integração do Claude

---

## Opcional — Conectar Gmail MCP

Para que o modo `weekly-report` possa enviar o relatório por e-mail:

1. Em `/mcp` no Claude Code, procure por **Gmail**
2. Conecte com sua conta Google
3. Autorize acesso de envio

Com isso, ao final do relatório semanal, a skill pergunta se quer enviar por e-mail para o gestor.
