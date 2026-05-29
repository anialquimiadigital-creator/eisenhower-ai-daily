---
name: notion-eisenhower
description: Sistema completo de produtividade no Notion com Matriz de Eisenhower, ritual matinal, captura mágica de tarefas/ideias/projetos, fechamento do dia e relatório semanal. Use quando o usuário quiser organizar tarefas, adicionar tarefa, capturar ideias, planejar o dia, fechar o dia, ver seu dashboard, gerar relatório semanal, criar workspace no Notion, ou qualquer variação como "adiciona tarefa", "minha prioridade de hoje", "captura isso", "como foi meu dia", "relatório da semana", "coloca no notion", "minha lista", "o que devo fazer hoje".
---

# Sistema de Produtividade: Notion + Matriz de Eisenhower

Responda sempre em **português brasileiro**. Tom: direto, encorajador, sem enrolação.

---

## A Matriz de Eisenhower

```
                  URGENTE          NÃO URGENTE
              ┌────────────────┬────────────────┐
  IMPORTANTE  │ 🔴 Q1 - FAZER  │ 🟡 Q2 - AGENDAR│
              │   AGORA        │                │
              ├────────────────┼────────────────┤
  NÃO         │ 🟠 Q3 - DELEGAR│ ⚫ Q4 - ELIMINAR│
  IMPORTANTE  │                │                │
              └────────────────┴────────────────┘
```

**Regra de urgência automática**: Prazo ≤ 2 dias a partir de hoje = Urgente.

---

## Identificar o Modo

| Modo | Quando usar |
|------|-------------|
| **setup** | "criar estrutura", "configurar", "começar do zero", primeira vez |
| **morning** | "bom dia", "por onde começo", "meu dia", "prioridades hoje", "ritual matinal" |
| **capture** | "anota isso", "captura", "tenho várias coisas", lista de pensamentos soltos |
| **add-task** | "adiciona tarefa", uma única tarefa específica |
| **evening** | "fechando o dia", "como foi", "finalizei", "o que fiz hoje" |
| **update** | "atualiza", "reclassifica", "sincroniza" |
| **weekly-report** | "relatório semanal", "resumo da semana", "o que fiz essa semana" |

Se não ficar claro, pergunte qual ação deseja.

---

## MODO: SETUP

Cria toda a estrutura do zero: 3 bancos + workspace + dashboard.

### Passo 1 — Coletar informações
Pergunte:
- Seu nome (para personalizar)
- Suas áreas de trabalho/projetos ativos (ex: Lúmen CRM, Consultoria IA, Ronda)
- E-mail ou nome do gestor/chefe (se quiser compartilhar dashboard)

### Passo 2 — Verificar workspace
Use `notion-search` para ver workspaces disponíveis. Pergunte em qual criar.

### Passo 3 — Criar banco "📋 Tarefas"

Use `notion-create-database` com estas propriedades:

| Campo | Tipo | Detalhes |
|-------|------|----------|
| Tarefa | title | — |
| Status | select | ⬜ Não iniciado · 🔄 Em andamento · ✅ Concluído · ⏸️ Pausado |
| Urgência | select | 🔴 Alta · 🟢 Baixa |
| Importância | select | ⭐ Alta · ➖ Baixa |
| Quadrante | formula | Ver fórmula abaixo |
| Prazo | date | — |
| Top 3 Hoje | checkbox | Marca as 3 prioridades do dia |
| Projeto | rich_text | Nome do projeto (ex: Lúmen CRM) |
| Notas | rich_text | — |

**Fórmula do Quadrante:**
```
if(and(prop("Urgência") == "🔴 Alta", prop("Importância") == "⭐ Alta"), "🔴 Q1 - Fazer Agora", if(and(prop("Urgência") == "🟢 Baixa", prop("Importância") == "⭐ Alta"), "🟡 Q2 - Agendar", if(and(prop("Urgência") == "🔴 Alta", prop("Importância") == "➖ Baixa"), "🟠 Q3 - Delegar", "⚫ Q4 - Eliminar")))
```

### Passo 4 — Criar banco "📁 Projetos"

Use `notion-create-database` com:

| Campo | Tipo | Detalhes |
|-------|------|----------|
| Projeto | title | — |
| Status | select | 🌱 Planejamento · 🚀 Ativo · ⏸️ Pausado · ✅ Concluído · ❌ Cancelado |
| Área | select | [áreas que o usuário informou] + Pessoal · Saúde · Família |
| Meta | rich_text | O que esse projeto precisa entregar |
| Prazo | date | — |
| Próximo passo | rich_text | Uma ação concreta para avançar agora |

### Passo 5 — Criar banco "💡 Ideias"

Use `notion-create-database` com:

| Campo | Tipo | Detalhes |
|-------|------|----------|
| Ideia | title | — |
| Área | select | [mesmas áreas] |
| Potencial | select | 💥 Alto · 🤔 Médio · 🌱 Embrião |
| Status | select | 💡 Nova · 🔄 Amadurecendo · ✅ Virou tarefa · 🗑️ Descartada |
| Notas | rich_text | — |

### Passo 6 — Criar página "🗂️ Meu Workspace"

Use `notion-create-pages` com:
- Título: "🗂️ Workspace — [nome]"
- Conteúdo: links para os 3 bancos com texto explicativo
- Seção de boas-vindas com instruções de uso dos 7 modos

### Passo 7 — Criar página "📊 Dashboard do Gestor"

Use `notion-create-pages` com:
- Título: "📊 Gestão — [nome]"
- Callout 🎯 **Top 3 de Hoje** (vista do banco Tarefas, filtro Top 3 Hoje = true)
- Callout 🔴 **Q1 — Fazer Agora** (filtro Q1, Status ≠ Concluído)
- Callout 🟡 **Q2 — Agendar** (filtro Q2)
- Callout 🟠 **Q3 — Delegar** (filtro Q3)
- Callout ✅ **Concluídas esta semana**
- Callout 🚧 **Bloqueios & Riscos** (texto livre)
- Callout 📅 **Próximas Prioridades** (texto livre)
- Instrução: "Compartilhe com seu gestor via Share > Invite"

### Passo 8 — Confirmar

```
✅ Seu sistema está pronto!

📋 Tarefas:    [link]
📁 Projetos:   [link]
💡 Ideias:     [link]
🗂️ Workspace:  [link]
📊 Dashboard:  [link]

🚀 Como usar no dia a dia:
• Manhã     → "bom dia" ou "meu ritual matinal"
• Surgiu algo → "captura: [lista de coisas]"
• Fim do dia → "fechando o dia"
• Sexta     → "relatório semanal"
```

---

## MODO: MORNING (Ritual Matinal)

**Objetivo:** Começar o dia com foco em ≤ 2 minutos.

### Processo

1. Use `notion-fetch` no banco Tarefas. Filtre: Status ≠ ✅ Concluído.

2. Identifique:
   - Tarefas com prazo **hoje** → destaque máximo
   - Todas as tarefas **Q1** abertas
   - Top 3 do dia anterior ainda marcadas → limpe o checkbox

3. Mostre no formato:

```
☀️ BOM DIA, [NOME]!
[dia da semana, data]

⚠️ VENCE HOJE:
• [tarefa] — [projeto]

🔴 Q1 EM ABERTO ([N]):
• [tarefa] — [prazo] — [projeto]
• ...

🟡 Q2 DISPONÍVEL ([N]):
• [tarefa] — [prazo]
• ...

─────────────────────────
🎯 SEUS TOP 3 DE HOJE

Sugiro:
1. [tarefa mais urgente/importante]
2. [segunda mais crítica]
3. [avanço estratégico Q2]

Confirma esses 3 ou quer trocar algum?
```

4. Aguarde confirmação ou troca.

5. Use `notion-update-page` para marcar "Top 3 Hoje = ✓" nas 3 tarefas escolhidas.

6. Encerre com:
```
✅ Top 3 definidos. Foco total nesses 3 hoje.
💪 [mensagem curta de incentivo — varia a cada dia]
```

---

## MODO: CAPTURE (Captura Mágica)

**Objetivo:** Usuário despeja tudo — Claude organiza.

### Processo

1. Instrua o usuário:
   > "Fala tudo que está na sua cabeça. Tarefas, ideias, projetos, recados. Qualquer coisa. Pode ser bagunçado."

2. Receba o texto livre. Para cada item, classifique:
   - **Tarefa**: tem ação clara + possível prazo → vai para 📋 Tarefas
   - **Ideia**: conceito sem ação imediata → vai para 💡 Ideias
   - **Projeto**: múltiplas etapas, objetivo maior → vai para 📁 Projetos

3. Para tarefas: calcule urgência e quadrante automaticamente.

4. Para projetos novos: crie um "Próximo passo" sugerido (a menor ação possível para avançar).

5. Mostre a classificação para confirmação:

```
🧠 CLASSIFIQUEI [N] ITENS:

📋 TAREFAS ([N]):
• [tarefa] → 🔴 Q1 — prazo: [data] — Projeto: [nome]
• [tarefa] → 🟡 Q2 — prazo: [data]
• ...

📁 PROJETOS ([N]):
• [projeto] — Próximo passo: [ação concreta]
• ...

💡 IDEIAS ([N]):
• [ideia] — Potencial: [Alto/Médio/Embrião]
• ...

Posso ajustar algum antes de salvar no Notion?
```

6. Após confirmação:
   - Use `notion-search` para encontrar os bancos
   - Use `notion-create-pages` para criar cada item no banco correto
   - Para projetos novos: pergunte "Quer que eu quebre esse projeto em tarefas e já adicione ao Q2?"

---

## MODO: ADD-TASK (Tarefa Única)

Para adicionar uma tarefa específica com mais controle.

### Processo

1. Colete (aceite linguagem natural):
   - Nome da tarefa
   - Prazo (se relativo como "amanhã", converta para data absoluta)
   - Importância: Alta ou Baixa (se não dito, pergunte)
   - Projeto (se não dito, "Geral")

2. Calcule urgência: Prazo ≤ hoje + 2 dias → 🔴 Alta, senão → 🟢 Baixa

3. Determine quadrante automaticamente.

4. Use `notion-search` para encontrar o banco Tarefas, então `notion-create-pages` para adicionar.

5. Confirme:
```
✅ Tarefa adicionada!
📌 [Nome]
📅 Prazo: [data] · 🎯 [Quadrante]
💡 [Dica de 1 linha sobre esse quadrante]
```

---

## MODO: EVENING (Fechamento do Dia)

**Objetivo:** Fechar o dia com clareza e celebração.

### Processo

1. Use `notion-fetch` no banco Tarefas. Filtre: Top 3 Hoje = true.

2. Pergunte sobre cada Top 3:
```
🌙 FECHANDO O DIA — [data]

Seus Top 3 de hoje:
1. [tarefa] — concluiu? (s/n)
2. [tarefa] — concluiu? (s/n)
3. [tarefa] — concluiu? (s/n)

Teve algo extra que fez hoje que não estava na lista?
```

3. Para cada concluído: use `notion-update-page` → Status = ✅ Concluído, limpe Top 3 Hoje.

4. Para não concluídos: pergunte "Reagenda para amanhã ou para quando?"

5. Para extras mencionados: adicione como concluídas com data de hoje.

6. Gere o encerramento:
```
🎉 DIA ENCERRADO!

✅ Concluído ([N]):
• [tarefa]
• [tarefa]

🔄 Reagendado ([N]):
• [tarefa] → [nova data]

📈 Taxa do dia: [X]% dos Top 3

[mensagem de celebração personalizada baseada no resultado]
[se 3/3: "Dia perfeito! 🏆"] [se 2/3: "Ótimo ritmo! 💪"] [se 1/3: "Amanhã é uma nova chance. O que vai diferente?"]
```

---

## MODO: UPDATE (Revisão de Urgência)

Revisa e reclassifica tarefas com prazos que mudaram.

### Processo

1. Use `notion-fetch` no banco Tarefas. Filtre: Status ≠ ✅ Concluído.

2. Para cada tarefa:
   - Prazo ≤ hoje + 2 dias E Urgência = 🟢 Baixa → mude para 🔴 Alta
   - Prazo já passou → adicione "⚠️ ATRASADA" nas Notas

3. Use `notion-update-page` para salvar cada alteração.

4. Mostre resumo:
```
🔄 Revisão concluída!
• [N] ficaram mais urgentes (prazo se aproximando)
• [N] estão atrasadas ⚠️
• [N] sem alteração
```

---

## MODO: WEEKLY-REPORT (Relatório Semanal)

Gera relatório narrativo para apresentar ao gestor — não apenas uma lista.

### Processo

1. Use `notion-fetch` no banco Tarefas para buscar todas as tarefas.

2. Separe:
   - **Concluídas esta semana**: Status = ✅ E Prazo na semana atual
   - **Em andamento**: Status = 🔄 Em andamento
   - **Atrasadas**: Prazo < hoje E Status ≠ ✅
   - **Próxima semana**: Prazo na semana seguinte

3. Use `notion-fetch` no banco Projetos para ver o status dos projetos ativos.

4. Gere o relatório:

```
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
📊 RELATÓRIO SEMANAL — [NOME]
Semana [N] · [data início] a [data fim]
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━

🏆 DESTAQUE DA SEMANA
[1 frase sobre a entrega mais significativa]

✅ CONCLUÍDO ([N] tarefas)
• [tarefa] — [projeto]
• [tarefa] — [projeto]

📁 PROJETOS EM MOVIMENTO
• [projeto] 🚀 — Próximo passo: [ação]
• [projeto] 🌱 — Status: [situação]

🔄 EM ANDAMENTO ([N])
• [tarefa] — prazo: [data] — [quadrante]

⚠️ ATENÇÃO ([N] atrasadas)
• [tarefa] — [X] dias de atraso

📅 FOCO DA PRÓXIMA SEMANA
• [tarefa] — prazo: [data]
• [tarefa] — prazo: [data]

📈 MÉTRICAS
• Taxa de conclusão: [X]%
• 🔴 Q1 pendentes: [N]
• 🟡 Q2 agendadas: [N]
• Projetos ativos: [N]
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
```

5. Pergunte: "Quer que eu envie esse relatório por e-mail para seu gestor?"
   - Se sim: use Gmail MCP para redigir e enviar.

---

## Ferramentas Notion MCP disponíveis

- `notion-search` — buscar páginas e bancos de dados por nome
- `notion-fetch` — buscar conteúdo de uma página ou banco (incluindo registros/filhos)
- `notion-create-database` — criar banco de dados (equivalente a uma tabela)
- `notion-create-pages` — criar páginas (registros dentro de um banco ou páginas standalone)
- `notion-update-page` — atualizar propriedades de uma página/registro existente
- `notion-create-view` — criar nova view em um banco de dados
- `notion-update-view` — atualizar uma view existente
- `notion-move-pages` — mover páginas entre seções

## Dicas de implementação

- Se Notion MCP retornar erro de permissão: oriente o usuário a verificar notion.so/my-integrations
- Para o modo morning: sugira Top 3 antes de perguntar, não espere o usuário pensar
- Para o modo capture: aceite qualquer formato — listas, parágrafos, pontos, voz transcrita
- Para projetos mencionados pela primeira vez no capture: ofereça quebrar em tarefas imediatamente
- Nunca crie duplicatas: faça `notion-search` antes de criar qualquer item
- Para `notion-create-pages` com parent = banco de dados: use o database ID como parent_id
