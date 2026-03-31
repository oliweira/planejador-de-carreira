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

Sinta-se livre para adaptar, traduzir ou integrar em sistemas maiores.
