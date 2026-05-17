# 🧬 Gémeo Digital do Tiago Rodrigues

**Tiago Simões Rodrigues** — 2022138676
Ciência de Dados para a Gestão · ISCAC / IPC · Cadeira de Fintech · 2025/2026

> Agente de inteligência artificial que me representa digitalmente — com base no meu currículo real, nos meus valores e na minha forma de comunicar, orientado para o domínio fintech.

**🌐 Demo ao vivo → [gemeo-digital.vercel.app](https://gemeo-digital.vercel.app)**

---

## O que é isto?

O **Gémeo Digital** é um chatbot de IA pessoal. Não é um assistente genérico — é uma representação digital autorizada de Tiago Simões Rodrigues, estudante de Ciência de Dados para a Gestão no ISCAC (Instituto Politécnico de Coimbra).

O agente responde com base no meu percurso real: a minha formação, a minha experiência profissional, os meus valores e os meus conhecimentos em fintech. Nunca inventa informação que não esteja documentada.

Desenvolvido para a cadeira de **Fintech** do ISCAC — 2025/2026.

---

## Como funciona?

O sistema tem **3 agentes** que trabalham em conjunto antes de cada resposta:

Pergunta do utilizador → Gémeo Digital → Subagente de Ética + Subagente de Psicologia → Resposta validada

### 👤 Gémeo Digital — Agente Principal
Responde como uma versão digital do Tiago. Conhece o meu percurso académico, experiência profissional, competências e valores. Actua como orquestrador dos outros dois agentes.

### ⚖️ Subagente de Ética & Compliance
Verifica cada resposta antes de chegar ao utilizador. Se detectar um problema, bloqueia a resposta automaticamente.

Normas verificadas:
- **RGPD** (Reg. 2016/679) — protecção de dados pessoais
- **EU AI Act** (Reg. 2024/1689) — IA de alto risco em serviços financeiros
- **MiFID II** (Dir. 2014/65/UE) — adequação de produtos de investimento
- **PSD2** (Dir. 2015/2366) — serviços de pagamento
- **AMLD6** (Dir. 2018/1673) — prevenção de branqueamento de capitais

Veredictos possíveis: `✅ Aprovado` · `⚠️ Aprovado com condições` · `❌ Vetado`

### 🧠 Subagente de Psicologia Comportamental
Analisa o tom da mensagem e adapta a resposta ao estado emocional do utilizador. Detecta enviesamentos cognitivos comuns em contexto financeiro:

| Enviesamento | O que é |
|---|---|
| Ancoragem | Fixação irracional num valor histórico |
| Aversão à perda | Medo de perder maior do que vontade de ganhar |
| Overconfidence | Excesso de confiança nas previsões próprias |
| Herding | Seguir a maioria sem pensar criticamente |
| Sunk Cost | Manter uma posição perdedora por inércia |
| Viés de recência | Decidir só com base nos últimos acontecimentos |

> O objectivo é sempre ajudar o utilizador a decidir melhor — nunca manipulá-lo.

---

## O que vês na dashboard

| Aba | Conteúdo |
|---|---|
| 💬 Conversa | Chat com o Gémeo Digital em tempo real |
| 📊 Dashboard | Métricas da sessão (verificações éticas, análises psicológicas) |
| 👤 Perfil | Currículo completo do Tiago |
| ℹ️ Sobre | Arquitectura do projecto e normas aplicadas |
| ⭐ Avaliador | Agente avaliador crítico para auto-avaliação do projecto |

Cada resposta inclui uma **faixa de validação ética**:

- 🟢 Verde — informação geral, verificação activa
- 🟡 Amarelo — risco elevado, consulta profissional recomendada
- 🔴 Vermelho — pedido recusado por incumprimento normativo

---

## Como usar

**1.** Cria uma chave gratuita em [console.groq.com](https://console.groq.com) → API Keys → Create API Key

**2.** Abre [gemeo-digital.vercel.app](https://gemeo-digital.vercel.app)

**3.** Cola a chave (começa por `gsk_...`) na janela que aparece e clica em **Activar**

**4.** Começa a conversar — a chave fica guardada no browser, só precisas de fazer isto uma vez

---

## Tecnologia

| Componente | Detalhe |
|---|---|
| Motor de IA | Llama 3.1 8B Instant via Groq API |
| Frontend | HTML5 + CSS3 + JavaScript puro |
| Deploy | Vercel — gratuito, sem servidor |
| Armazenamento | localStorage do browser |

Sem frameworks. Sem dependências externas. Um único ficheiro HTML.

---

## Skills criadas

**🔍 [Ethics Compliance Checker](skills/ethics-compliance-checker.md)**
Verificador normativo automático para agentes de IA em serviços financeiros. Cobre RGPD, MiFID II, EU AI Act, PSD2 e AMLD6.

**📊 [Behavioral Finance Analyzer](skills/behavioral-finance-analyzer.md)**
Detecção de enviesamentos cognitivos financeiros em sistemas conversacionais. Baseado em Kahneman & Tversky, Deci & Ryan e Thaler & Sunstein.

**👤 [Personal Identity Skill](skills/personal-identity-skill.md)**
Guia para construir um agente com identidade pessoal verificável, ancorada num perfil real documentado.

**⭐ [Critical Evaluator Skill](skills/critical-evaluator-skill.md)**
Agente avaliador crítico académico para auto-avaliação de projectos de IA. Identifica pontos fracos, atribui notas fundamentadas e antecipa perguntas difíceis.

---

## Documentação

- 📄 [Relatório Final](Relatorio_Final_Gemeo_Digital.pdf)
- 🧬 [System Prompt](system-prompt.md)
- 📋 [Changelog](CHANGELOG.md)

---

*Representação digital autorizada. O agente nunca se apresenta como o Tiago real.*
