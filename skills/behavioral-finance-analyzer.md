# 🧠 Behavioral Finance Analyzer

Skill de detecção de enviesamentos cognitivos financeiros e adaptação comportamental para agentes de IA conversacionais.

---

## O que é e porque é inovador

A literacia financeira é baixa na maioria das populações europeias — e mesmo quem tem formação financeira toma decisões influenciadas por enviesamentos cognitivos. Os chatbots financeiros actuais ignoram este problema: respondem da mesma forma independentemente do estado emocional ou cognitivo do utilizador.

Esta skill resolve esse problema com um mecanismo que lê o estado do utilizador antes de responder e adapta a comunicação para facilitar decisões mais racionais. A inovação está em três aspectos:

1. **Detecção passiva** — o utilizador não precisa de declarar o seu estado; o sistema infere-o a partir da linguagem natural
2. **Adaptação comunicacional** — não apenas o conteúdo, mas o tom, o ritmo e a estrutura da resposta mudam com base no perfil detectado
3. **Ética do nudge** — os mecanismos de influência são usados exclusivamente para benefício do utilizador, não da instituição

---

## Quando usar

- Em agentes de apoio a decisões de investimento, poupança ou crédito
- Em sistemas de aconselhamento financeiro pessoal
- Em chatbots de gestão de dívida ou recuperação financeira
- Em qualquer sistema onde o estado emocional do utilizador possa comprometer a qualidade da decisão
- Em ferramentas de educação financeira adaptativa

---

## Enviesamentos cognitivos detectados

| Enviesamento | Definição | Sinal linguístico típico | Risco financeiro |
|---|---|---|---|
| **Ancoragem** | Fixação num valor de referência inicial que distorce decisões futuras | "Comprei a 50€, não vendo abaixo disso" | Recusa de saída de posições perdedoras por comparação ao preço de entrada |
| **Aversão à perda** | A dor de perder é psicologicamente mais intensa do que o prazer de ganhar o mesmo valor | "Não quero arriscar perder nada" | Sub-optimização crónica de retornos; excesso de activos sem risco |
| **Overconfidence** | Excesso de confiança nas próprias previsões e capacidades de análise | "Vai subir de certeza", "Eu sei o que estou a fazer" | Concentração excessiva de risco; ausência de diversificação |
| **Herding** | Decisões baseadas no comportamento da maioria, sem avaliação crítica independente | "Toda a gente está a comprar X" | Exposição a bolhas especulativas; compra em topos de mercado |
| **Sunk Cost Fallacy** | Manutenção de posições ou projectos por causa do que já foi investido, não pelo valor futuro esperado | "Já investi demasiado para sair agora" | Aprofundamento de perdas; má alocação de recursos |
| **Hyperbolic Discounting** | Preferência irracional pelo presente sobre o futuro, desproporcionalmente maior do que o valor temporal do dinheiro justificaria | "Preciso do dinheiro já, não me interessa o longo prazo" | Sacrifício de objectivos de longo prazo por gratificação imediata |
| **Viés de recência** | Atribuição de peso excessivo a eventos recentes na avaliação de tendências | "O mercado subiu 3 meses seguidos, vai continuar" | Comprar topos; vender fundos; desconsiderar séries históricas |

---

## Estados emocionais analisados e adaptações

| Estado | Sinais detectados | Risco de decisão | Adaptação recomendada |
|---|---|---|---|
| **Stress financeiro agudo** | Urgência, "preciso agora", deadlines, linguagem de desespero | Decisões impulsivas e irreversíveis | Tom calmo, validação emocional, sugestão de pausa antes de agir |
| **Ansiedade** | Pedidos repetidos de confirmação, catastrofização, perguntas sobre o pior cenário | Paralisia ou decisões excessivamente conservadoras | Estrutura clara, ritmo lento, âncoras de estabilidade, foco no controlável |
| **Euforia** | Certezas absolutas, resistência ao downside, linguagem de "oportunidade única" | Concentração excessiva de risco, desconsideração de cenários adversos | Tom neutro, introdução gradual de perspectivas contrárias |
| **Calmo e informado** | Linguagem factual, horizonte temporal longo, pedido de comparação de opções | Baixo — estado ideal para decisão | Tom técnico, apresentação equilibrada de opções e trade-offs |
| **Vergonha financeira** | Minimização de problemas, resistência a revelar valores reais | Sub-reporte de problemas, atraso em procurar ajuda | Tom não-julgamental, normalização, foco em soluções |

---

## Fundamentos teóricos

| Autor / Obra | Contribuição para esta skill |
|---|---|
| Kahneman & Tversky (1979) — *Prospect Theory* | Base matemática da aversão à perda; função de valor assimétrica; pesos de probabilidade distorcidos |
| Kahneman (2011) — *Thinking, Fast and Slow* | Distinção entre Sistema 1 (rápido, emocional) e Sistema 2 (lento, racional); heurísticas e enviesamentos cognitivos |
| Thaler & Sunstein (2008) — *Nudge* | Arquitectura de escolha ética; defaults como instrumento de bem-estar; nudging sem manipulação |
| Deci & Ryan (1985) — *Self-Determination Theory* | Motivação intrínseca; linguagem autonomia-suportativa; importância de preservar a sensação de controlo |
| Shefrin & Statman (1985) — *The Disposition Effect* | Tendência para vender ganhos cedo e manter perdas demasiado tempo |

---

## Como implementar em qualquer agente

**Passo 1 — Define o perfil de análise no system prompt**

```
SUPERVISÃO PSICOLÓGICA ACTIVA:
Para cada mensagem do utilizador, analisa:
- Estado emocional provável: calmo | ansioso | stressado | eufórico | envergonhado
- Enviesamentos activos: lista com evidência textual da mensagem
- Nível de literacia financeira estimado: básico | intermédio | avançado
- Necessidade de simplificação, empatia ou validação adicional
```

**Passo 2 — Define as adaptações de resposta**

```
Com base na análise, ajusta:
- Tom: técnico | neutro | empático | calmo | validador
- Nível de detalhe: simplificado | intermédio | técnico
- O que enfatizar: autonomia | reversibilidade | alternativas | riscos
- O que evitar: linguagem de urgência | certezas absolutas | pressão
```

**Passo 3 — Define os limites éticos**

```
LIMITES INVIOLÁVEIS:
- Nunca usar nudges para benefício da instituição ou do agente
- Nunca efectuar diagnósticos clínicos ou psicológicos formais
- Nunca reduzir a autonomia do utilizador — só apoiá-la
- Em caso de dúvida entre nudge e neutralidade, opta pela neutralidade
- Sinais de fragilidade financeira grave → sugerir apoio humano qualificado
```

---

## Diferença entre manipulação e nudging ético

| | Manipulação | Nudging Ético |
|---|---|---|
| **Objectivo** | Benefício da instituição | Benefício do utilizador |
| **Transparência** | Oculta | Pode ser revelada sem perda de eficácia |
| **Autonomia** | Reduz | Preserva e reforça |
| **Reversibilidade** | Dificulta mudança de decisão | Facilita reconsideração |
| **Conformidade EU AI Act** | Proibido (Art. 5) | Permitido e encorajado |

---

## Reutilização em outros contextos

| Contexto | Adaptação necessária |
|---|---|
| Saúde e bem-estar | Substituir enviesamentos financeiros por enviesamentos de saúde (optimismo irrealista, negação) |
| Educação | Adaptar para enviesamentos de aprendizagem (efeito Dunning-Kruger, aversão ao esforço) |
| RH e carreira | Adaptar para enviesamentos de avaliação de desempenho e tomada de decisão profissional |
| E-commerce | Detectar compras impulsivas e estados de ansiedade de consumo |

---

## Referências

- Kahneman, D. & Tversky, A. (1979). Prospect Theory: An Analysis of Decision under Risk. *Econometrica*, 47(2), 263–291
- Kahneman, D. (2011). *Thinking, Fast and Slow*. Farrar, Straus and Giroux
- Thaler, R. H. & Sunstein, C. R. (2008). *Nudge: Improving Decisions About Health, Wealth, and Happiness*. Yale University Press
- Deci, E. L. & Ryan, R. M. (1985). *Intrinsic Motivation and Self-Determination in Human Behavior*. Plenum Press
- Shefrin, H. & Statman, M. (1985). The Disposition to Sell Winners Too Early and Ride Losers Too Long. *Journal of Finance*, 40(3), 777–790

---

*Skill desenvolvida no âmbito do projecto Gémeo Digital — Cadeira de Fintech, ISCAC/IPC, 2025/2026.*
