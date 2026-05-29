# ⚡ Os 7 Modos da Skill

A skill `notion-eisenhower` detecta automaticamente o que você quer fazer a partir da linguagem natural. Você não precisa digitar um comando exato — só falar o que precisa.

---

## Modo 1 — `setup` — Configuração inicial

**Como ativar:** "criar minha estrutura", "configurar", "começar do zero"

Cria toda a estrutura no Notion automaticamente. Você só precisa responder 3 perguntas:
- Seu nome
- Suas áreas de trabalho ou projetos ativos
- Nome ou e-mail do seu gestor (opcional)

**O que é criado:**

| Banco/Página | O que é |
|---|---|
| 📋 Tarefas | Banco principal com quadrantes, Top 3, prazo e projeto |
| 📁 Projetos | Banco de projetos com meta e próximo passo |
| 💡 Ideias | Banco de captura livre sem pressão de prazo |
| 🗂️ Workspace | Sua área privada com links para tudo |
| 📊 Dashboard | Página para compartilhar com seu gestor |

**Tempo:** 3–5 minutos. Após isso, você nunca mais precisa configurar nada.

---

## Modo 2 — `morning` — Ritual Matinal

**Como ativar:** "bom dia", "por onde começo", "prioridades hoje", "meu dia"

O modo mais poderoso do sistema. Você abre o Claude de manhã, digita "bom dia", e recebe em segundos:

```
☀️ BOM DIA, ANELISE!
quinta-feira, 29 de maio

⚠️ VENCE HOJE:
• Enviar proposta Lúmen — Consultoria IA

🔴 Q1 EM ABERTO (2):
• Revisar contrato Hub Geriatria — prazo: amanhã
• Responder e-mail cliente X — prazo: hoje

🟡 Q2 DISPONÍVEL (4):
• Criar conteúdo para Instagram — prazo: sexta
• ...

─────────────────────────
🎯 SEUS TOP 3 DE HOJE

Sugiro:
1. Enviar proposta Lúmen (vence hoje)
2. Revisar contrato Hub Geriatria (vence amanhã)
3. Criar conteúdo Instagram (Q2 estratégico)

Confirma esses 3 ou quer trocar algum?
```

Você confirma ou ajusta. A skill marca os 3 no Notion e manda uma mensagem de foco para começar.

**Tempo:** 2 minutos.

---

## Modo 3 — `capture` — Captura Mágica

**Como ativar:** "captura:", "anota isso", "tenho várias coisas"

O modo para esvaziar a cabeça. Você despeja tudo em texto livre — bagunçado, sem ordem, como vier — e a skill organiza.

**Exemplo de entrada:**
```
captura: reunião com cliente Lúmen amanhã às 14h urgente, 
ideia de fazer um mini-curso de produtividade com IA, 
preciso ligar pro contador essa semana, 
projeto novo: criar pacote de consultoria para ILPIs, 
comprar presente da minha mãe semana que vem
```

**Saída da skill:**
```
🧠 CLASSIFIQUEI 5 ITENS:

📋 TAREFAS (3):
• Reunião com cliente Lúmen → 🔴 Q1 — prazo: amanhã — Projeto: Lúmen CRM
• Ligar pro contador → 🟡 Q2 — prazo: essa semana
• Comprar presente da mãe → 🟡 Q2 — prazo: semana que vem — Pessoal

📁 PROJETOS (1):
• Pacote de consultoria para ILPIs — Próximo passo: definir escopo e precificação

💡 IDEIAS (1):
• Mini-curso de produtividade com IA — Potencial: Alto

Posso ajustar algum antes de salvar no Notion?
```

Você confirma e tudo vai para o Notion de uma vez.

---

## Modo 4 — `add-task` — Tarefa Única

**Como ativar:** "adiciona tarefa", "cria uma task", tarefa específica com detalhes

Para quando você quer adicionar uma tarefa com mais controle. Aceita linguagem natural:

> "Adiciona tarefa: revisar apresentação do cliente, prazo sexta, muito importante, projeto Lúmen"

A skill calcula a urgência pelo prazo, determina o quadrante e confirma:

```
✅ Tarefa adicionada!
📌 Revisar apresentação do cliente
📅 Prazo: sexta-feira, 30/05 · 🟡 Q2 - Agendar
💡 Q2: bloqueia tempo para isso antes que vire urgência.
```

---

## Modo 5 — `evening` — Fechamento do Dia

**Como ativar:** "fechando o dia", "como foi", "finalizei", "encerrando"

Fecha o dia com clareza e celebração. A skill busca seus Top 3 do dia e pergunta o que foi feito:

```
🌙 FECHANDO O DIA — quinta, 29/05

Seus Top 3 de hoje:
1. Enviar proposta Lúmen — concluiu? (s/n)
2. Revisar contrato Hub Geriatria — concluiu? (s/n)
3. Criar conteúdo Instagram — concluiu? (s/n)

Teve algo extra que fez hoje que não estava na lista?
```

Após suas respostas:

```
🎉 DIA ENCERRADO!

✅ Concluído (2):
• Enviar proposta Lúmen
• Revisar contrato Hub Geriatria

🔄 Reagendado (1):
• Criar conteúdo Instagram → amanhã, sexta

📈 Taxa do dia: 67% dos Top 3

Ótimo ritmo! Dois de três é consistência que acumula. 💪
```

---

## Modo 6 — `update` — Revisão de Urgência

**Como ativar:** "atualiza", "reclassifica", "sincroniza", "revisa urgências"

Percorre todas as tarefas abertas e atualiza automaticamente:
- Tarefas com prazo chegando (≤ 2 dias) que ainda estão em Q2 → promovidas para Q1
- Tarefas com prazo vencido → marcadas com ⚠️ ATRASADA

```
🔄 Revisão concluída!
• 2 ficaram mais urgentes (prazo se aproximando)
• 1 está atrasada ⚠️
• 8 sem alteração
```

Recomendado: rodar uma vez por semana ou quando sentir que a lista perdeu o foco.

---

## Modo 7 — `weekly-report` — Relatório Semanal

**Como ativar:** "relatório semanal", "resumo da semana", "o que fiz essa semana"

Gera um relatório narrativo completo — não uma lista fria, mas uma visão real da semana:

```
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
📊 RELATÓRIO SEMANAL — ANELISE
Semana 22 · 26/05 a 30/05
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━

🏆 DESTAQUE DA SEMANA
Proposta Lúmen CRM enviada e aprovada — maior avanço comercial do mês.

✅ CONCLUÍDO (7 tarefas)
• Proposta Lúmen CRM — Consultoria IA
• Reunião Hub Geriatria — Hub Geriatria
• ...

📁 PROJETOS EM MOVIMENTO
• Lúmen CRM 🚀 — Próximo passo: onboarding do cliente
• Consultoria IA 🌱 — Status: proposta enviada, aguardando retorno

🔄 EM ANDAMENTO (3)
• Criar conteúdo Instagram — prazo: sexta — Q2

⚠️ ATENÇÃO (1 atrasada)
• Atualizar site — 3 dias de atraso

📅 FOCO DA PRÓXIMA SEMANA
• Onboarding Lúmen CRM — prazo: terça
• Criar conteúdo Instagram — prazo: sexta

📈 MÉTRICAS
• Taxa de conclusão: 78%
• 🔴 Q1 pendentes: 1
• 🟡 Q2 agendadas: 4
• Projetos ativos: 3
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
```

Ao final, pergunta se quer enviar por e-mail para o gestor.

---

## Resumo rápido

| Diga isso | Modo ativado |
|---|---|
| "bom dia" | morning |
| "captura: [lista]" | capture |
| "adiciona tarefa X" | add-task |
| "fechando o dia" | evening |
| "atualiza urgências" | update |
| "relatório semanal" | weekly-report |
| "criar minha estrutura" | setup |
