# 📋 Guia de Montagem Manual no Notion

Sem precisar de Claude Code, programação ou qualquer configuração técnica. Você cria os 3 bancos abaixo no Notion e usa os quadrantes manualmente. Tempo estimado: **20–30 minutos**.

Funciona em qualquer plano do Notion, incluindo o gratuito.

---

## O que você vai criar

```
📋 Tarefas        ← banco principal com a Matriz de Eisenhower
📁 Projetos       ← banco de projetos vinculados às tarefas
💡 Ideias         ← captura de ideias sem pressão de prazo
📊 Dashboard      ← página para visualizar tudo e compartilhar com gestor
```

---

## Banco 1 — 📋 Tarefas

### Como criar

1. No Notion, clique em **+ New page**
2. Escolha o tipo **Database — Full page**
3. Nomeie como `📋 Tarefas`

### Colunas a criar

| Nome | Tipo | Opções |
|------|------|--------|
| Tarefa | Title | — |
| Status | Select | ⬜ Não iniciado · 🔄 Em andamento · ✅ Concluído · ⏸️ Pausado |
| Urgência | Select | 🔴 Alta · 🟢 Baixa |
| Importância | Select | ⭐ Alta · ➖ Baixa |
| Quadrante | Select | 🔴 Q1 - Fazer Agora · 🟡 Q2 - Agendar · 🟠 Q3 - Delegar · ⚫ Q4 - Eliminar |
| Prazo | Date | — |
| Top 3 Hoje | Checkbox | — |
| Projeto | Text | Nome do projeto |
| Notas | Text | — |

> **Dica:** o campo Quadrante é preenchido manualmente — use a tabela abaixo como referência rápida.

### Tabela de referência dos quadrantes

| Urgência | Importância | Quadrante |
|----------|-------------|-----------|
| 🔴 Alta | ⭐ Alta | 🔴 Q1 - Fazer Agora |
| 🟢 Baixa | ⭐ Alta | 🟡 Q2 - Agendar |
| 🔴 Alta | ➖ Baixa | 🟠 Q3 - Delegar |
| 🟢 Baixa | ➖ Baixa | ⚫ Q4 - Eliminar |

**Regra de urgência:** qualquer tarefa com prazo em até 2 dias = Urgência Alta automaticamente.

---

## Banco 2 — 📁 Projetos

### Como criar

1. Crie uma nova página do tipo **Database — Full page**
2. Nomeie como `📁 Projetos`

### Colunas a criar

| Nome | Tipo | Opções |
|------|------|--------|
| Projeto | Title | — |
| Status | Select | 🌱 Planejamento · 🚀 Ativo · ⏸️ Pausado · ✅ Concluído · ❌ Cancelado |
| Área | Select | [suas áreas: ex. Marketing, Financeiro, Operações, Pessoal] |
| Meta | Text | O que esse projeto precisa entregar |
| Prazo | Date | — |
| Próximo passo | Text | Uma ação concreta para avançar agora |

---

## Banco 3 — 💡 Ideias

### Como criar

1. Crie uma nova página do tipo **Database — Full page**
2. Nomeie como `💡 Ideias`

### Colunas a criar

| Nome | Tipo | Opções |
|------|------|--------|
| Ideia | Title | — |
| Área | Select | [mesmas áreas dos Projetos] |
| Potencial | Select | 💥 Alto · 🤔 Médio · 🌱 Embrião |
| Status | Select | 💡 Nova · 🔄 Amadurecendo · ✅ Virou tarefa · 🗑️ Descartada |
| Notas | Text | — |

> **Como usar:** qualquer coisa que surgir na cabeça vai aqui — sem julgamento, sem prazo, sem pressão. Uma vez por semana você revisa e decide o que vira tarefa ou projeto.

---

## Página — 📊 Dashboard

### Como criar

1. Crie uma **New page** normal (não database)
2. Nomeie como `📊 Dashboard — [seu nome]`
3. Configure as seções abaixo

### Estrutura da página

**Seção 1 — Callout: 🎯 Top 3 de Hoje**
- Adicione um Linked View do banco Tarefas
- Filtro: Top 3 Hoje = ✓
- Esta seção mostra só as 3 prioridades do dia

**Seção 2 — Callout: 🔴 Q1 — Fazer Agora**
- Adicione um Linked View do banco Tarefas
- Filtros: Quadrante = "🔴 Q1 - Fazer Agora" E Status ≠ "✅ Concluído"

**Seção 3 — Callout: 🟡 Q2 — Agendar**
- Linked View com filtro: Quadrante = "🟡 Q2 - Agendar" E Status ≠ "✅ Concluído"

**Seção 4 — Callout: 🟠 Q3 — Delegar**
- Linked View com filtro: Quadrante = "🟠 Q3 - Delegar" E Status ≠ "✅ Concluído"

**Seção 5 — Callout: ✅ Concluídas esta semana**
- Linked View com filtro: Status = "✅ Concluído" E Prazo = Esta semana

**Seção 6 — Texto livre: 🚧 Bloqueios & Riscos**
- Escreva manualmente o que está impedindo seu avanço

**Seção 7 — Texto livre: 📅 Foco da Próxima Semana**
- Escreva as 2–3 prioridades da próxima semana

> **Para compartilhar com o gestor:** Share → Invite → adicione o e-mail dele como "Can view"

---

## Ritual de uso diário (sem IA)

| Momento | O que fazer |
|---------|-------------|
| **Manhã (5 min)** | Abrir o banco Tarefas → marcar Top 3 Hoje → começar pelo Q1 |
| **Durante o dia** | Qualquer coisa nova → Captura direto no banco correto (Tarefas, Projetos ou Ideias) |
| **Fim do dia (5 min)** | Marcar o que foi concluído → desmarcar Top 3 Hoje → reagendar o que ficou |
| **Sexta-feira (15 min)** | Revisar semana → atualizar urgências → planejar próxima semana |

---

## Dicas rápidas

- **Nunca deixe uma tarefa sem quadrante.** Se não sabe onde colocar, é Q2 ou Q4.
- **Top 3 é rígido.** Máximo 3. Se quiser adicionar uma 4ª, retire uma das outras.
- **Ideias não são tarefas.** Não coloque prazo, não classifique — só capture.
- **Revise os projetos uma vez por semana.** Atualize o "Próximo passo" sempre que avançar.
- **Quando tudo parece Q1**, revise com calma. A maioria é Q3 ou Q4 com pressa dos outros.
