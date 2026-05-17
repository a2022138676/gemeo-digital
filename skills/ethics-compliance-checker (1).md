# ⚖️ Ethics Compliance Checker

Skill de verificação normativa automática para agentes de IA em serviços financeiros e domínios regulados.

---

## O que é e porque é inovador

A maioria dos agentes de IA em serviços financeiros não tem qualquer mecanismo de verificação ética activo — respondem com aparente confiança mesmo quando violam normas regulatórias europeas. Esta skill resolve esse problema com um árbitro normativo interno que opera antes de cada resposta, de forma transparente e auditável.

A inovação está em três aspectos:

1. **Verificação antes da resposta** — o agente não responde e depois pede desculpa. Bloqueia antes.
2. **Veredicto incontornável** — um veto não pode ser sobreposto pelo agente principal, eliminando o risco de contorno.
3. **Visibilidade para o utilizador** — o resultado da verificação é mostrado com código de cores, materializando o princípio de transparência do EU AI Act.

---

## Quando usar

- Em qualquer agente de IA que responda a questões financeiras, de investimento ou crédito
- Em chatbots de onboarding bancário, seguros ou gestão de património
- Em sistemas de apoio à decisão com dados pessoais de utilizadores
- Em qualquer contexto onde a conformidade com regulação europeia seja obrigatória ou esperada

---

## Quadro normativo coberto

| Norma | Âmbito | Artigos relevantes |
|---|---|---|
| **RGPD** — Reg. 2016/679 | Protecção de dados pessoais, decisão automatizada com efeitos jurídicos | Art. 5, 6, 22 |
| **EU AI Act** — Reg. 2024/1689 | IA de alto risco em serviços financeiros: transparência, supervisão humana, robustez | Art. 9, 10, 13, 14, 15 |
| **MiFID II** — Dir. 2014/65/UE | Adequação de produtos de investimento, conflitos de interesse, melhor interesse do cliente | Art. 24, 25 |
| **PSD2** — Dir. 2015/2366 | Protecção do consumidor em pagamentos digitais, Open Banking | Art. 66, 67 |
| **AMLD6** — Dir. 2018/1673 | Prevenção de branqueamento de capitais, KYC/AML, transacções suspeitas | Art. 3, 6, 7 |

---

## Sistema de veredictos

| Veredicto | Condição | Acção | Indicador visual |
|---|---|---|---|
| ✅ **Aprovado** | Resposta conforme com todas as normas | Entregue sem alterações | Faixa verde |
| ⚠️ **Aprovado com condições** | Risco identificado, mitigação possível | Entregue com aviso e recomendação de profissional | Faixa amarela |
| ❌ **Vetado** | Violação normativa grave | Resposta bloqueada, utilizador informado | Faixa vermelha |

**O veredicto Vetado é absolutamente incontornável.** O agente principal não pode sobrepô-lo em nenhuma circunstância — esta é a garantia estrutural de conformidade do sistema.

---

## Condições de veto absoluto

Qualquer pedido que contenha os seguintes elementos resulta automaticamente em Vetado:

- Evasão fiscal, fraude ou branqueamento de capitais
- Uso de características protegidas (raça, género, religião) como critério de decisão financeira
- Promessa explícita de lucros, rentabilidades ou resultados garantidos
- Acesso ou exposição de dados pessoais privados sem base legal
- Manipulação ou pressão sobre o utilizador para tomar decisões irreversíveis
- Violação dos requisitos de transparência do EU AI Act (Art. 13)

---

## Como implementar em qualquer agente

**Passo 1 — Incorpora as normas no system prompt**

```
SUPERVISÃO ÉTICA ACTIVA:
Antes de cada resposta financeira ou sensível, verifica:
- Promete lucros ou resultados garantidos? → VETADO
- Usa dados pessoais sem base legal? → VETADO
- Incentiva risco desproporcional ao perfil? → APROVADO COM CONDIÇÕES
- É transparente e explicável? → APROVADO
- Envolve pedido de natureza ilegal? → VETADO
```

**Passo 2 — Define o output estruturado**

```
O subagente devolve:
- veredicto: APROVADO | APROVADO_COM_CONDICOES | VETADO
- normas_verificadas: lista das normas consultadas
- flags: lista de problemas detectados (se existirem)
- justificacao: razão do veredicto em linguagem clara
```

**Passo 3 — Integra no agente principal**

O agente principal recebe o veredicto, aplica-o e adapta a resposta antes de enviar ao utilizador. Em caso de Vetado, substitui a resposta por uma mensagem de recusa em linguagem respeitosa.

**Passo 4 — Torna o resultado visível**

Mostra o resultado da verificação ao utilizador com indicador visual — não apenas internamente. A transparência é um requisito do EU AI Act e um factor de confiança para o utilizador.

---

## Reutilização em outros contextos

Esta skill foi desenvolvida para fintech mas é directamente aplicável em:

| Sector | Adaptação necessária |
|---|---|
| Seguros | Adicionar Dir. Solvência II e IDD |
| Crédito ao consumo | Adicionar Dir. Crédito Imobiliário |
| Gestão de activos | Reforçar Art. 24-25 MiFID II |
| Saúde digital | Substituir por RGPD + MDR (Reg. 2017/745) |
| Recursos humanos | Substituir por RGPD + Dir. Igualdade de Tratamento |

---

## Impacto na confiança do utilizador

Sistemas que mostram activamente os seus mecanismos de verificação ética geram maior confiança do que sistemas que apenas declaram ser éticos. Esta skill implementa o princípio de **transparência operacional** — não basta dizer que se cumpre a regulação; é preciso mostrar que se cumpre, em cada resposta, de forma verificável.

---

## Referências

- Parlamento Europeu e Conselho (2024). Regulamento (UE) 2024/1689 — EU AI Act
- Parlamento Europeu e Conselho (2016). Regulamento (UE) 2016/679 — RGPD
- Parlamento Europeu e Conselho (2014). Directiva 2014/65/UE — MiFID II
- European Banking Authority (2020). Guidelines on ICT and security risk management
- Financial Stability Board (2017). Artificial Intelligence and Machine Learning in Financial Services

---

*Skill desenvolvida no âmbito do projecto Gémeo Digital — Cadeira de Fintech, ISCAC/IPC, 2025/2026.*
