# 🧠 Behavioral Finance Analyzer

Skill de detecção de enviesamentos cognitivos financeiros para sistemas conversacionais de IA.

---

## O que faz?

Analisa o conteúdo e o tom de cada mensagem do utilizador, identifica padrões cognitivos que podem distorcer a qualidade das suas decisões financeiras, e fornece ao agente principal recomendações de adaptação comunicacional.

Não efectua diagnósticos clínicos. Actua exclusivamente como consultor interno de comunicação — o seu objectivo é facilitar a autonomia decisional do utilizador, nunca substituí-la nem manipulá-la.

---

## Quando usar esta skill?

- Em agentes de apoio a decisões de investimento ou poupança
- Em sistemas de aconselhamento financeiro pessoal
- Em chatbots de crédito ou gestão de dívida
- Em qualquer sistema onde o estado emocional do utilizador possa afectar a qualidade da decisão

---

## Enviesamentos cognitivos detectados

| Enviesamento | Sinal linguístico típico | Risco financeiro |
|---|---|---|
| **Ancoragem** | "Comprei a X€, não vendo abaixo disso" | Decisões de saída distorcidas pelo preço de entrada |
| **Aversão à perda** | Recusa de risco mesmo quando matematicamente justificado | Sub-optimização crónica de retornos |
| **Overconfidence** | "Vai subir de certeza" | Concentração excessiva de risco |
| **Herding** | "Toda a gente está a comprar X" | Exposição a bolhas especulativas |
| **Sunk Cost** | "Já investi demasiado para sair agora" | Manutenção de posições perdedoras |
| **Hyperbolic Discounting** | Preferência marcada por liquidez imediata | Sacrifício de objectivos de longo prazo |
| **Viés de recência** | Decisões baseadas nos últimos 3 a 6 meses | Comprar topos, vender fundos |

---

## Estados emocionais analisados

| Estado | Sinais detectados | Adaptação recomendada |
|---|---|---|
| **Stress financeiro** | Urgência, "preciso agora", deadline | Tom mais calmo, validação emocional primeiro |
| **Ansiedade** | Pedidos repetidos de confirmação, catastrofização | Estrutura clara, ritmo lento, âncoras de estabilidade |
| **Euforia** | Certezas absolutas, resistência ao downside | Tom neutro, introdução suave de cenários adversos |
| **Calmo** | Linguagem factual, horizonte temporal longo | Tom técnico, apresentação de opções e trade-offs |

---

## Fundamentos teóricos

| Autor | Obra | Contribuição |
|---|---|---|
| Kahneman e Tversky | Prospect Theory (1979) | Aversão à perda, framing effects, pesos de probabilidade |
| Kahneman | Thinking, Fast and Slow (2011) | Sistema 1 vs Sistema 2, heurísticas e enviesamentos |
| Deci e Ryan | Self-Determination Theory (1985) | Motivação intrínseca, linguagem autonomia-suportativa |
| Thaler e Sunstein | Nudge (2008) | Arquitectura de escolha ética, defaults, framing positivo |

---

## Como implementar

**Passo 1 — Define o perfil psicográfico no system prompt**

Instrui o agente a analisar, para cada mensagem do utilizador, o estado emocional provável, os enviesamentos activos com evidência textual, o nível de literacia financeira estimado e a necessidade de simplificação ou empatia adicional.

**Passo 2 — Estrutura o output**

O subagente devolve um perfil estruturado com o estado emocional, a intensidade, os enviesamentos detectados e as recomendações de tom, nível técnico e o que enfatizar ou evitar na resposta.

**Passo 3 — Integra no agente principal**

O agente principal recebe o perfil e ajusta o tom, a estrutura e o nível de detalhe da resposta antes de a enviar ao utilizador.

---

## Princípios éticos de aplicação

- **Não manipulação** — os nudges sugeridos são sempre para benefício do utilizador, nunca da instituição
- **Não diagnóstico** — identifica padrões comportamentais, não patologias
- **Privacidade cognitiva** — as inferências são internas ao sistema, nunca partilhadas com terceiros
- **Humildade epistémica** — possível enviesamento detectado não equivale a enviesamento confirmado
- **Autonomia** — em caso de dúvida entre um nudge e neutralidade, opta pela neutralidade

---

## Referências

- Kahneman, D. e Tversky, A. (1979). Prospect Theory: An Analysis of Decision under Risk
- Thaler, R. e Sunstein, C. (2008). Nudge: Improving Decisions About Health, Wealth, and Happiness
- Deci, E. e Ryan, R. (1985). Intrinsic Motivation and Self-Determination in Human Behavior

---

*Skill desenvolvida no âmbito do projecto Gémeo Digital — Cadeira de Fintech, ISCAC/IPC, 2025/2026.*
