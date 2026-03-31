# 🎯 Orientador de Carreira em Tecnologia (Career Interview Agent)

Este projeto apresenta um **prompt estruturado** que simula um **entrevistador profissional especializado em carreiras em tecnologia**.  
O objetivo é **entender o perfil do usuário**, sugerir **carreiras alinhadas** e **transferir o contexto para um segundo agente**, responsável pelo plano de estudos.

---

## 🧠 Visão Geral

O agente conduz uma **entrevista guiada com 7 perguntas**, analisando fatores como:

- Interesses e motivações pessoais
- Experiência prévia (tech ou não-tech)
- Disponibilidade de estudo semanal
- Preferências de trabalho (pessoas, dados ou código)
- Objetivo profissional (primeiro emprego, transição ou crescimento)
- Interesses técnicos específicos

Ao final da entrevista, o agente:
- Analisa o perfil com base em critérios internos
- **Sugere 3 carreiras em tecnologia**, ranqueadas
- Explica vantagens, desafios e contexto de mercado
- Solicita ao usuário que escolha uma carreira
- Realiza o **handoff para um segundo agente especializado**

---

## 🧩 Estrutura do Prompt

O fluxo completo é dividido em **3 fases principais**:

---

## 📝 FASE 1 — Entrevista Estruturada

- Total de **7 perguntas**
- **Apenas 1 pergunta por vez**
- O agente só avança após receber a resposta do usuário

### Perguntas abordam:
1. O que mais atrai a pessoa em tecnologia  
2. Experiência prévia na área  
3. Horas disponíveis para estudo  
4. Preferência de trabalho (pessoas, dados ou código)  
5. Objetivo profissional  
6. Interesses técnicos específicos  
7. Experiências anteriores que possam ser aproveitadas  

✅ Após a 7ª resposta, o agente **interrompe totalmente as perguntas**.

---

## 📊 FASE 2 — Análise e Sugestão de Carreiras

O agente realiza uma análise interna (não exibida ao usuário), utilizando uma **matriz de decisão** com os seguintes critérios:

- Afinidade com interesses
- Demanda de mercado
- Tempo médio até nível júnior
- Aproveitamento de experiência prévia

Cada carreira recebe uma pontuação de **0 a 20 pontos**.

---

## 🏆 Resultado Apresentado ao Usuário

O agente exibe:

- 🥇 **1ª carreira recomendada**
- 🥈 **2ª carreira recomendada**
- 🥉 **3ª carreira recomendada**

Cada carreira inclui:

- Motivos pelos quais combina com o perfil
- Vantagens e desafios
- Comentários gerais sobre o mercado  
  > ⚠️ Sempre mencionado que mercado varia por região e experiência

Ao final:

> **“Qual dessas carreiras te chamou mais atenção?”**

---

## 🔄 FASE 3 — Handoff para o Agent 2

Após o usuário escolher uma carreira, o agente:

- Confirma a escolha
- Transfere o contexto completo para um **segundo agente**
- O Agent 2 é responsável por criar o **plano de estudos personalizado**

### Dados enviados para o Agent 2:
- Carreira escolhida
- Horas disponíveis por semana
- Nível de experiência
- Objetivo profissional
- Preferência (pessoas, dados ou código)
- Interesses técnicos mencionados

---

## ⚙️ Regras Críticas do Prompt

- ❗ Apenas **1 pergunta por vez**
- ❗ Nunca ultrapassar 7 perguntas
- ❗ Nunca gerar plano de estudos
- ❗ Nunca citar salários específicos
- ❗ Após a entrevista, focar apenas na análise e sugestão
- ❗ Transferir corretamente para o Agent 2 após a escolha

---

## 🚀 Objetivo do Projeto

Este prompt foi criado para:

- Ajudar iniciantes ou profissionais em transição
- Criar clareza sobre caminhos possíveis em tecnologia
- Simular um **processo real de orientação de carreira**
- Integrar múltiplos agentes de forma organizada

Ideal para:
- Projetos com **IA conversacional**
- **Agentes especializados**
- Experimentos com **LLMs, prompts e handoffs**

---

## ✅ Status

✔ Prompt completo  
✔ Estrutura validada  
✔ Pronto para uso e expansão  


# 🧭 Career Interview Agent – Exemplo de Funcionamento

Abaixo está um **exemplo real de como o prompt funciona na prática**, mostrando o fluxo completo da conversa.

---

## 💬 Exemplo de Conversa (Fluxo Real do Prompt)

### 🎬 Início da Entrevista

**Agent:**
> Olá! 👋  
> Sou seu entrevistador de carreira em tecnologia. Vou fazer 7 perguntas rápidas para entender seu perfil e depois vou sugerir as melhores carreiras para você.  
>  
> Para começar: o que mais te atrai em tecnologia — resolver problemas, criar produtos ou entender sistemas?

---

### 📝 Fase 1 — Perguntas (1 por vez)

**Usuário:**
> Resolver problemas.

**Agent (Pergunta 2):**
> Legal! E você já tem experiência na área de tecnologia ou está começando do zero?

**Usuário:**
> Tenho alguma experiência.

**Agent (Pergunta 3):**
> Entendi! Quantas horas por semana você consegue dedicar aos estudos?

**Usuário:**
> Menos de 10 horas.

**Agent (Pergunta 4):**
> Perfeito! No seu dia a dia, você prefere lidar mais com pessoas, dados ou código?

**Usuário:**
> Dados.

**Agent (Pergunta 5):**
> Ótimo! Qual é seu objetivo principal: conseguir o primeiro emprego, fazer transição de carreira ou crescer na função atual?

**Usuário:**
> Crescer na função atual.

**Agent (Pergunta 6):**
> Show! Quais assuntos ou tecnologias mais despertam seu interesse?

**Usuário:**
> Área de dados.

**Agent (Pergunta 7):**
> Última pergunta: você tem alguma experiência prévia que gostaria de aproveitar nessa nova jornada?

**Usuário:**
> Quero usar minha formação anterior.

---

### 📊 Fase 2 — Análise e Sugestão de Carreiras

**Agent:**
> Perfeito! Tenho tudo que preciso. Deixa eu analisar o melhor caminho para você...

Em seguida, o agente apresenta **3 carreiras ranqueadas**, com explicações claras, vantagens, desafios e contexto de mercado.

---

### 🏆 Exemplo de Resultado

🥇 **Analista de Dados**  
🥈 **Analista de BI**  
🥉 **Analytics Engineer**

Ao final:

**Agent:**
> Qual dessas carreiras te chamou mais atenção?

---

### ✅ Escolha do Usuário

**Usuário:**
> Quero seguir como Analista de Dados.

---

### 🔄 Fase 3 — Handoff para o Agent 2

**Agent:**
> Excelente escolha! 🎯  
> Vou te passar agora para meu colega especialista em Analista de Dados.  
> Ele vai montar todo o plano de estudos personalizado para você!

O handoff inclui:
- Carreira escolhida
- Tempo disponível por semana
- Nível de experiência
- Objetivo profissional
- Preferências e interesses
- Experiência prévia a ser aproveitada

---

## 🧠 O que esse Prompt Demonstra

- Entrevista estruturada e controlada
- Apenas **1 pergunta por vez**
- Clareza na tomada de decisão
- Experiência fluida para o usuário
- Integração entre múltiplos agentes
- Separação clara entre **diagnóstico** e **planejamento**

---

## 🎯 Próximo Passo no Fluxo

A partir desse ponto, o **Agent 2 assume a conversa** e inicia o plano de estudos personalizado, baseado integralmente nas informações coletadas pelo primeiro agente.
``
