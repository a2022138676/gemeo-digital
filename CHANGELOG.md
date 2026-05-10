# Changelog — Gémeo Digital do Tiago Rodrigues

Registo de todas as versões e alterações do projecto.

---

## [1.3] — Maio 2026

### Corrigido
- Lógica de verificação ética corrigida — o badge vermelho passava a disparar
  erradamente quando o agente mencionava palavras como "fraude" ou "branqueamento"
  nas suas respostas explicativas. A verificação passou a analisar apenas a
  mensagem do utilizador, não a resposta do agente.
- Adicionado retry automático em caso de rate limit da API Groq — o sistema
  aguarda o tempo necessário e reenvia o pedido sem intervenção do utilizador.

---

## [1.2] — Maio 2026

### Alterado
- Modelo de linguagem trocado de `llama-3.3-70b-versatile` para
  `llama-3.1-8b-instant` para reduzir consumo de tokens por minuto
  e evitar erros de limite de taxa no plano gratuito.
- Tokens máximos por resposta reduzidos de 1024 para 800.

---

## [1.1] — Maio 2026

### Corrigido
- Ficheiro renomeado de `gemeo-digital final.html` para `index.html`
  para ser servido correctamente pela Vercel na raiz do domínio.

### Adicionado
- Deploy automático na Vercel a partir do repositório GitHub.
- URL permanente: gemeo-digital.vercel.app

---

## [1.0] — Maio 2026

### Lançamento inicial

- Agente principal configurado com system prompt completo baseado
  no perfil real de Tiago Simões Rodrigues.
- Subagente de Ética e Moral implementado — verifica conformidade
  com RGPD, MiFID II, EU AI Act, PSD2 e AMLD6 antes de cada resposta.
- Subagente de Psicologia Comportamental implementado — detecta
  enviesamentos cognitivos financeiros e adapta o tom da comunicação.
- Dashboard web com quatro abas: Conversa, Dashboard, Perfil e Sobre.
- Indicadores visuais de validação ética em tempo real (verde, amarelo,
  vermelho) por baixo de cada resposta.
- Autenticação via chave Groq guardada em localStorage — sem servidor,
  sem custos de infraestrutura.
- Modelo inicial: Llama 3.3 70B Versatile via Groq API.

---

*Projecto desenvolvido para a cadeira de Fintech — ISCAC/IPC, 2025/2026.*
