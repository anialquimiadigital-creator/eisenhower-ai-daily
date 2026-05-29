---
name: notion-eisenhower
description: Sistema completo de produtividade com Matriz de Eisenhower integrado ao Notion e Google Calendar. Gerencia tarefas, projetos, ideias e compromissos de agenda. Use quando o usuário quiser organizar tarefas, adicionar tarefa, capturar ideias ou compromissos, planejar o dia, fechar o dia, ver relatório semanal, adicionar evento na agenda, ou qualquer variação como "adiciona tarefa", "minha prioridade de hoje", "captura isso", "como foi meu dia", "coloca na agenda", "marca no calendario", "relatório da semana", "o que devo fazer hoje".
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

## Lógica de Classificação

Use esta seção para classificar qualquer tarefa **sem precisar perguntar** para o usuário. Só pergunte quando o contexto for genuinamente ambíguo.

### O que é URGENTE 🔴

Marque urgente quando **qualquer** uma destas condições for verdadeira:
- Prazo ≤ 2 dias (regra automática)
- Cliente ativo esperando resposta (especialmente >12h sem retorno)
- Está bloqueando outra pessoa de trabalhar
- Oportunidade com janela de tempo (proposta prestes a vencer, evento hoje/amanhã)
- Compromisso já marcado que precisa de preparo imediato

### O que é IMPORTANTE ⭐

Marque importante quando a tarefa:
- Afeta diretamente receita (cliente pagante, entrega de projeto, cobrança, proposta)
- Avança um projeto ativo (Ronda, Cardápio IA, Consultoria IA, Palestras Daltro)
- Impacta reputação ou posicionamento (qualidade de entrega, palestra, conteúdo estratégico)
- Previne problema maior futuro (processo, documentação, saúde, relacionamento chave)
- É estratégica para o crescimento do negócio (mesmo sem prazo)
- Envolve saúde ou família (exceto burocracia rotineira)

Marque **não importante** quando:
- Outra pessoa pode fazer igualmente bem
- Resultado não afeta nenhum objetivo real
- É burocracia ou tarefa administrativa rotineira
- É distração disfarçada de tarefa

### Regras por tipo de tarefa

| Tipo de tarefa | Quadrante padrão | Exceção |
|---|---|---|
| Entrega para cliente ativo | 🔴 Q1 | Se prazo distante → 🟡 Q2 |
| Responder cliente (mensagem/e-mail) | 🟠 Q3 | Se aguarda >12h ou é decisão → 🔴 Q1 |
| Montar/enviar proposta | 🔴 Q1 | Se está só iniciando → 🟡 Q2 |
| Reunião/compromisso hoje ou amanhã | 🔴 Q1 | — |
| Reunião planejada (>2 dias) | 🟡 Q2 | — |
| Criar conteúdo / marketing | 🟡 Q2 | Se tem deadline hoje → 🔴 Q1 |
| Estudar / desenvolver habilidade | 🟡 Q2 | — |
| Planejamento estratégico | 🟡 Q2 | — |
| Saúde preventiva (consulta, exame) | 🟡 Q2 | Se sintoma agudo → 🔴 Q1 |
| Financeiro: pagamento vencendo | 🔴 Q1 | — |
| Financeiro: planejamento / DRE | 🟡 Q2 | — |
| Tarefas administrativas rotineiras | 🟠 Q3 | — |
| Responder mensagens de rotina | 🟠 Q3 | — |
| Organizar arquivos / pastas | 🟠 Q3 ou ⚫ Q4 | Se bloqueia trabalho → 🟠 Q3 |
| Scroll, reunião sem pauta, burocracia inútil | ⚫ Q4 | — |

### Regras por área (contexto ANi)

| Área | Importância padrão | Raciocínio |
|---|---|---|
| Consultoria IA | ⭐ Alta | Afeta receita e reputação diretamente |
| Projeto Ronda (ILPI) | ⭐ Alta | Projeto ativo com cliente real |
| Cardápio IA | ⭐ Alta | Projeto ativo com cliente real |
| IA e Palestras Daltro | ⭐ Alta | Posicionamento e receita |
| Pessoal | ⭐ Alta se bem-estar/família · ➖ Baixa se burocracia | Avalie caso a caso |
| Saúde | ⭐ Alta | Sempre importante, urgência depende da situação |
| Família | ⭐ Alta | Sempre importante |

### Perguntas de desempate (use quando ambíguo)

1. **"Alguém está esperando isso de você hoje?"** → Sim = urgente
2. **"Se não fizer essa semana, tem consequência real?"** → Sim = importante
3. **"Isso avança algum projeto ativo ou gera receita?"** → Sim = importante
4. **"Outra pessoa poderia fazer isso no seu lugar?"** → Sim = Q3 (delegar)
5. **"Se você tirar isso da lista, alguém vai notar?"** → Não = Q4 (eliminar)

### Sinais de reclassificação automática

- "responder" + pessoa aleatória → 🟠 Q3 (não Q1)
- "responder" + cliente ativo + urgente → 🔴 Q1
- "reunião" + hoje/amanhã → 🔴 Q1 independente do tema
- "criar" / "desenvolver" / "planejar" → 🟡 Q2 salvo deadline imediato
- "organizar" / "arrumar" / "limpar" → 🟠 Q3 ou ⚫ Q4
- "estudar" / "aprender" / "ler" → 🟡 Q2
- qualquer tarefa sem prazo E sem impacto em projeto ativo → 🟡 Q2 ou ⚫ Q4

---

## Identificar o Modo

| Modo | Quando usar |
|------|-------------|
| **setup** | "criar estrutura", "configurar", "começar do zero", primeira vez |
| **morning** | "bom dia", "por onde começo", "meu dia", "prioridades hoje", "ritual matinal" |
| **capture** | "anota isso", "captura", "tenho várias coisas", lista de pensamentos soltos |
| **add-task** | "adiciona tarefa", uma única tarefa específica |
| **add-event** | "coloca na agenda", "marca no calendário", "agendar", evento com horário específico |
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
| Área | select | [áreas que o usuário informou] + Pessoal · Saúde · Família |
| Projeto | rich_text | Nome do projeto (ex: Lúmen CRM) |
| Notas | rich_text | — |

**Fórmula do Quadrante:**
```
if(and(prop("Urgência") == "🔴 Alta", prop("Importância") == "⭐ Alta"), "🔴 Q1 - Fazer Agora", if(and(prop("Urgência") == "🟢 Baixa", prop("Importância") == "⭐ Alta"), "🟡 Q2 - Agendar", if(and(prop("Urgência") == "🔴 Alta", prop("Importância") == "➖ Baixa"), "🟠 Q3 - Delegar", "⚫ Q4 - Eliminar")))
```

Após criar o banco, use `notion-create-view` para adicionar estas views extras:

| View | Tipo | Configuração |
|------|------|-------------|
| 🗂️ Matriz | board | Agrupado por Quadrante · filtro Status ≠ Concluído |
| 📅 Calendário | calendar | Por campo Prazo · mostra Tarefa + Quadrante |
| 📊 Cronograma | timeline | Por campo Prazo · agrupado por Área |

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
| Tarefas | relation | Relacionar com o banco Tarefas criado no Passo 3 |
| Progresso | rollup | Fonte: relação Tarefas · propriedade: Status · cálculo: % de valores que são "✅ Concluído" |

Após criar o banco, use `notion-create-view` para adicionar:

| View | Tipo | Configuração |
|------|------|-------------|
| 📊 Cronograma | timeline | Por campo Prazo · filtro Status ≠ Concluído · mostra Projeto + Progresso |

### Passo 5 — Criar banco "💡 Ideias"

Use `notion-create-database` com:

| Campo | Tipo | Detalhes |
|-------|------|----------|
| Ideia | title | — |
| Área | select | [mesmas áreas] |
| Potencial | select | 💥 Alto · 🤔 Médio · 🌱 Embrião |
| Status | select | 💡 Nova · 🔄 Amadurecendo · ✅ Virou tarefa · 🗑️ Descartada |
| Notas | rich_text | — |

### Passo 6 — Criar Hub Pessoal "🗂️ [nome] — Workspace"

Esta é a página de uso pessoal diário. Use `notion-create-pages` para criar com o layout abaixo.

**Estrutura da página (de cima para baixo):**

**Bloco 1 — Menu de navegação**
Crie um banco de dados galeria inline chamado "Menu" com cards de navegação:

| Card | Ícone |
|------|-------|
| Tarefas | ✅ |
| Projetos | 📁 |
| Ideias | 💡 |
| Agenda | 📅 |
| Metas | 🎯 |
| Relatório | 📊 |

Configure cada card com link para o banco ou página correspondente.

**Bloco 2 — Agenda de hoje (largura total)**
Callout com ícone 📅 e texto em negrito **Agenda de Hoje**. Instrução ao executar o setup: deixar este bloco como texto livre — será preenchido automaticamente no modo morning com os eventos do Google Calendar do dia.

**Bloco 3 — Grade 2×2 dos quadrantes**
Duas linhas de 2 colunas cada (use layout columns do Notion):

Linha 1:
- Coluna esquerda: callout vermelho 🔴 **Q1 — Fazer Agora** com view inline do banco Tarefas filtrada por Quadrante = "🔴 Q1 - Fazer Agora" e Status ≠ Concluído
- Coluna direita: callout amarelo 🟡 **Q2 — Agendar** com view inline filtrada por Quadrante = "🟡 Q2 - Agendar" e Status ≠ Concluído

Linha 2:
- Coluna esquerda: callout laranja 🟠 **Q3 — Delegar** com view inline filtrada por Quadrante = "🟠 Q3 - Delegar" e Status ≠ Concluído
- Coluna direita: callout cinza ⚫ **Q4 — Eliminar** com view inline filtrada por Quadrante = "⚫ Q4 - Eliminar" e Status ≠ Concluído

**Bloco 4 — Projetos e Ideias (2 colunas)**
- Coluna esquerda: callout 📁 **Projetos Ativos** com view inline do banco Projetos filtrada por Status = "🚀 Ativo"
- Coluna direita: callout 💡 **Ideias em Alta** com view inline do banco Ideias filtrada por Potencial = "💥 Alto"

### Passo 7 — Criar página "📊 Dashboard — [nome]"

Esta página é para o dono do negócio ou gestor acompanhar o que está em andamento. Layout limpo: apenas a grade 2×2 da Matriz de Eisenhower, sem menu, sem extras.

Use `notion-create-pages` com:
- Título: "📊 Dashboard — [nome]"

**Estrutura da página — grade 2×2 pura:**

Linha 1 (2 colunas):
- Coluna esquerda: callout vermelho 🔴 **Q1 — Fazer Agora** (urgente + importante) com view inline do banco Tarefas filtrada por Quadrante = "🔴 Q1 - Fazer Agora" e Status ≠ Concluído · exibe: Tarefa, Prazo, Projeto, Área
- Coluna direita: callout amarelo 🟡 **Q2 — Agendar** (importante, não urgente) com view inline filtrada por Quadrante = "🟡 Q2 - Agendar" e Status ≠ Concluído · exibe: Tarefa, Prazo, Projeto

Linha 2 (2 colunas):
- Coluna esquerda: callout laranja 🟠 **Q3 — Delegar** (urgente, não importante) com view inline filtrada por Quadrante = "🟠 Q3 - Delegar" e Status ≠ Concluído · exibe: Tarefa, Prazo, Projeto
- Coluna direita: callout cinza ⚫ **Q4 — Eliminar** (nem urgente nem importante) com view inline filtrada por Quadrante = "⚫ Q4 - Eliminar" e Status ≠ Concluído · exibe: Tarefa, Projeto

Após criar a página, instrua: "Compartilhe este dashboard com o dono do negócio via Share → Invite no Notion."

### Passo 8 — Confirmar

```
✅ Seu sistema está pronto!

📋 Tarefas:    [link]
📁 Projetos:   [link]
💡 Ideias:     [link]
🗂️ Workspace:  [link]  ← seu hub pessoal diário
📊 Dashboard:  [link]  ← compartilhe com o dono do negócio

🚀 Como usar no dia a dia:
• Manhã       → "bom dia" ou "meu ritual matinal"
• Surgiu algo → "captura: [lista de coisas]"
• Fim do dia  → "fechando o dia"
• Sexta       → "relatório semanal"
```

---

## MODO: MORNING (Ritual Matinal)

**Objetivo:** Começar o dia com foco em ≤ 2 minutos.

### Processo

1. Em paralelo, busque:
   - `notion-fetch` no banco Tarefas (Status ≠ ✅ Concluído)
   - `google-calendar-list-events` com startTime = início do dia atual e endTime = fim do dia atual (timeZone: America/Sao_Paulo)

2. Identifique nas tarefas:
   - Tarefas com prazo **hoje** → destaque máximo
   - Todas as tarefas **Q1** abertas
   - Top 3 do dia anterior ainda marcadas → limpe o checkbox

3. Mostre no formato:

```
☀️ BOM DIA, [NOME]!
[dia da semana, data]

📅 SUA AGENDA DE HOJE:
• [horário] — [evento]
• [horário] — [evento]
(se não houver eventos: "Agenda livre hoje!")

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

Sugiro (considerando seus compromissos de agenda):
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
   - **Tarefa**: tem ação clara + possível prazo, sem horário fixo → vai para 📋 Tarefas (Notion)
   - **Evento/Compromisso**: tem horário específico OU é recorrente (reunião, consulta, aula, voluntariado, rotina pessoal) → vai para 📅 Google Calendar
   - **Ideia**: conceito sem ação imediata → vai para 💡 Ideias (Notion)
   - **Projeto**: múltiplas etapas, objetivo maior → vai para 📁 Projetos (Notion)

   **Regra de ouro para Evento vs Tarefa:** se tem hora marcada ou repete com frequência fixa → Calendar. Se é uma ação a executar sem horário específico → Tarefas.

3. Para tarefas: classifique urgência e importância **automaticamente** usando a seção "Lógica de Classificação" acima. Não pergunte — decida. Só pergunte se o contexto for genuinamente impossível de inferir.

4. Para projetos novos: crie um "Próximo passo" sugerido (a menor ação possível para avançar).

5. Mostre a classificação para confirmação:

```
🧠 CLASSIFIQUEI [N] ITENS:

📋 TAREFAS ([N]) → Notion:
• [tarefa] → 🔴 Q1 — prazo: [data] — Projeto: [nome]
• [tarefa] → 🟡 Q2 — prazo: [data]
• ...

📅 AGENDA ([N]) → Google Calendar:
• [evento] — [dia/horário] — [recorrente? sim/não]
• ...

📁 PROJETOS ([N]) → Notion:
• [projeto] — Próximo passo: [ação concreta]
• ...

💡 IDEIAS ([N]) → Notion:
• [ideia] — Potencial: [Alto/Médio/Embrião]
• ...

Posso ajustar algum antes de salvar?
```

6. Após confirmação:
   - Tarefas/Projetos/Ideias: use `notion-search` + `notion-create-pages` nos bancos corretos
   - Eventos: use `google-calendar-create-event` com os campos:
     - summary: nome do evento
     - startTime / endTime: horários no formato ISO 8601
     - timeZone: "America/Sao_Paulo"
     - recurrenceData: ["RRULE:FREQ=WEEKLY;BYDAY=FR"] para recorrentes semanais, ["RRULE:FREQ=WEEKLY;BYDAY=MO,WE,FR"] para múltiplos dias, etc.
     - overrideReminders: [{"method": "popup", "minutes": 30}] como padrão
   - **Tarefas Q1/Q2 com Prazo**: além de salvar no Notion, crie também um lembrete no Google Calendar:
     - summary: "📌 [nome da tarefa]"
     - startTime: Prazo às 09:00, endTime: Prazo às 09:30
     - timeZone: "America/Sao_Paulo"
     - overrideReminders: Q1 → 1440 min antes (1 dia) · Q2 → 4320 min antes (3 dias)
   - Para projetos novos: pergunte "Quer que eu quebre esse projeto em tarefas e já adicione ao Q2?"

---

## MODO: ADD-EVENT (Evento na Agenda)

Para adicionar um compromisso com horário específico ou recorrente ao Google Calendar.

### Processo

1. Colete (aceite linguagem natural):
   - Nome do evento
   - Data e horário de início e fim
   - Local (opcional)
   - Recorrência (toda semana? todo mês? dias específicos?)

2. Para recorrência, mapeie:
   - "toda semana na [dia]" → RRULE:FREQ=WEEKLY;BYDAY=[XX]
   - "toda segunda e quarta" → RRULE:FREQ=WEEKLY;BYDAY=MO,WE
   - "todo mês no dia X" → RRULE:FREQ=MONTHLY;BYMONTHDAY=X
   - "uma vez só" → sem recorrência

3. Use `google-calendar-create-event` com timeZone: "America/Sao_Paulo"

4. Confirme:
```
✅ Evento criado na agenda!
📅 [Nome do evento]
🕐 [horário início] às [horário fim]
📍 [local, se informado]
🔁 [Recorrência ou "Único"]
🔔 Lembrete: 30 min antes
```

---

## MODO: ADD-TASK (Tarefa Única)

Para adicionar uma tarefa específica com mais controle.

### Processo

1. Colete (aceite linguagem natural):
   - Nome da tarefa
   - Prazo (se relativo como "amanhã", converta para data absoluta)
   - Projeto/Área (se não dito, infira pelo contexto)

2. Classifique **automaticamente** usando a seção "Lógica de Classificação":
   - Urgência: prazo ≤ 2 dias → 🔴 Alta; ou use os sinais contextuais da tarefa
   - Importância: use as regras por tipo de tarefa e por área (ANi)
   - Não pergunte — decida. Só pergunte se for genuinamente impossível inferir.

3. Determine quadrante automaticamente.

4. Use `notion-search` para encontrar o banco Tarefas, então `notion-create-pages` para adicionar.

5. **Sincronizar com Google Calendar** — se a tarefa tem Prazo E é Q1 ou Q2:
   - Use `google-calendar-create-event` com:
     - summary: "📌 [nome da tarefa]"
     - startTime: Prazo às 09:00, endTime: Prazo às 09:30
     - timeZone: "America/Sao_Paulo"
     - overrideReminders:
       - Q1 → `[{"method": "popup", "minutes": 1440}]` (1 dia antes)
       - Q2 → `[{"method": "popup", "minutes": 4320}]` (3 dias antes)
   - Q3 e Q4: não criar evento no Calendar (não justifica espaço na agenda)

6. Confirme:
```
✅ Tarefa adicionada!
📌 [Nome]
📅 Prazo: [data] · 🎯 [Quadrante]
📆 Lembrete criado no Google Calendar: [data] às 9h
💡 [Dica de 1 linha sobre esse quadrante]
```
Se não tem prazo, omita a linha do Calendar.

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

## Ferramentas disponíveis

### Notion MCP
- `notion-search` — buscar páginas e bancos de dados por nome
- `notion-fetch` — buscar conteúdo de uma página ou banco (incluindo registros/filhos)
- `notion-create-database` — criar banco de dados (equivalente a uma tabela)
- `notion-create-pages` — criar páginas (registros dentro de um banco ou páginas standalone)
- `notion-update-page` — atualizar propriedades de uma página/registro existente
- `notion-create-view` — criar nova view em um banco de dados
- `notion-update-view` — atualizar uma view existente
- `notion-move-pages` — mover páginas entre seções

### Google Calendar MCP
- `google-calendar-create-event` — criar evento (único ou recorrente via RRULE)
- `google-calendar-list-events` — listar eventos de um período (use para morning mode)
- `google-calendar-update-event` — atualizar evento existente
- `google-calendar-delete-event` — remover evento
- `google-calendar-list-calendars` — listar calendários disponíveis

**Timezone padrão:** sempre usar `America/Sao_Paulo` em todos os eventos.
**RRULE dias:** MO=segunda, TU=terça, WE=quarta, TH=quinta, FR=sexta, SA=sábado, SU=domingo.

## Dicas de implementação

- Se Notion MCP retornar erro de permissão: oriente o usuário a verificar notion.so/my-integrations
- Para o modo morning: sugira Top 3 antes de perguntar, não espere o usuário pensar
- Para o modo capture: aceite qualquer formato — listas, parágrafos, pontos, voz transcrita
- Para projetos mencionados pela primeira vez no capture: ofereça quebrar em tarefas imediatamente
- Nunca crie duplicatas: faça `notion-search` antes de criar qualquer item
- Para `notion-create-pages` com parent = banco de dados: use o database ID como parent_id
- **Sincronização Calendar**: toda tarefa Q1 ou Q2 com Prazo gera automaticamente um lembrete no Google Calendar. Q3 e Q4 não geram — não justificam espaço na agenda. Se a tarefa não tem prazo, não criar evento.
- **Não duplicar eventos**: se o item já foi classificado como Evento (vai para o Calendar com horário), não criar também como tarefa no Notion. São destinos diferentes.
