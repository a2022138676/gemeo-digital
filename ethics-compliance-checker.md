# ⚖️ Ethics Compliance Checker

Skill de verificação normativa automática para agentes de IA em serviços financeiros.

---

## O que faz?

Avalia cada resposta de um agente de IA antes de ser entregue ao utilizador, verificando se está em conformidade com o quadro regulatório europeu aplicável a serviços financeiros. Se detetar um problema, bloqueia ou condiciona a resposta automaticamente.

Não comunica com o utilizador — actua exclusivamente nos bastidores, como um auditor interno.

---

## Quando usar esta skill?

- Sempre que um agente de IA responda a questões financeiras
- Em sistemas de apoio à decisão de investimento ou crédito
- Em chatbots de onboarding bancário ou seguros
- Em qualquer sistema que processe dados pessoais de utilizadores

---

## Normas verificadas

| Norma | Descrição |
|---|---|
| **RGPD** — Reg. 2016/679 | Protecção de dados pessoais e direito à explicação de decisões automatizadas (Art. 22) |
| **EU AI Act** — Reg. 2024/1689 | Sistemas de IA de alto risco em serviços financeiros: transparência, supervisão humana e robustez |
| **MiFID II** — Dir. 2014/65/UE | Adequação de produtos de investimento e obrigação de actuar no melhor interesse do cliente |
| **PSD2** — Dir. 2015/2366 | Protecção do consumidor em serviços de pagamento e Open Banking |
| **AMLD6** — Dir. 2018/1673 | Prevenção do branqueamento de capitais e financiamento do terrorismo (KYC/AML) |

---

## Veredictos possíveis

| Veredicto | Significado | Acção |
|---|---|---|
| Aprovado | Resposta conforme | Entregue ao utilizador sem alterações |
| Aprovado com condições | Flags detetados, mitigação possível | Entregue com aviso de risco |
| Vetado | Violação normativa grave | Resposta bloqueada, utilizador informado |

Um veredicto **Vetado é incontornável** — o agente principal não pode sobrepô-lo.

---

## Condições de veto absoluto

- Pedidos com características de branqueamento de capitais
- Uso de características protegidas como critério de decisão (raça, género, religião)
- Evidência de manipulação ou pressão sobre o utilizador
- Violação de normas imperativas do EU AI Act (Art. 9–15)
- Promessas de lucros ou rentabilidades garantidas

---

## Como implementar

**Passo 1 — Define o contexto normativo no system prompt**

Instrui o agente a verificar antes de cada resposta financeira se existe promessa de lucros garantidos, uso de dados pessoais sem base legal, incentivo a risco desproporcional ou falta de transparência.

**Passo 2 — Estrutura o output**

O subagente devolve um veredicto estruturado com as normas verificadas, os flags detetados e a justificação da decisão.

**Passo 3 — Integra no agente principal**

O agente principal recebe o veredicto, aplica-o e adapta a resposta antes de a enviar ao utilizador.

---

## Indicadores visuais recomendados

- Verde — Aprovado, informação de carácter geral
- Amarelo — Aprovado com condições, risco elevado
- Vermelho — Vetado, pedido recusado

---

## Referências

- EU AI Act — Reg. 2024/1689 — eur-lex.europa.eu
- RGPD — Reg. 2016/679 — eur-lex.europa.eu
- MiFID II — Dir. 2014/65/UE — eur-lex.europa.eu

---

*Skill desenvolvida no âmbito do projecto Gémeo Digital — Cadeira de Fintech, ISCAC/IPC, 2025/2026.*
