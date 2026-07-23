# Agente Local — ReAct Demo 🤖

**PT-BR** | [English below](#local-agent--react-demo)

Um mini-agente que roda **100% no navegador**, sem LLM e sem chamadas externas. Ele recebe um objetivo em linguagem natural e simula o loop **ReAct** (Reasoning + Acting): **Pensar → Agir → Observar**, mostrando cada passo numa timeline em tempo real. As ferramentas (`search`, `calculator`, `write_file`) são todas simuladas em JavaScript.

### ✨ Features

- Loop ReAct completo visualizado passo a passo (Pensamento, Ação, Observação, Resposta final)
- Três ferramentas mockadas: busca, calculadora (avaliação aritmética real e segura) e gravação de arquivo
- Planner que interpreta o objetivo (detecta números, intenção de busca e de escrita)
- Interface bilíngue PT/EN com toggle instantâneo
- Exemplos clicáveis para começar rápido
- Arquivo único `index.html`, sem dependências, sem build, sem `localStorage`

### ▶️ Como usar

1. Abra o `index.html` em qualquer navegador moderno.
2. Digite um objetivo (ex.: *"Calcule 15% de 240"*) ou clique num exemplo.
3. Clique em **Executar agente** e acompanhe os passos do agente na timeline.
4. Use o botão **PT / EN** para trocar o idioma.

### 🧠 Como funciona

O `planSteps(goal)` transforma o objetivo num roteiro de passos ReAct. Cada intenção detectada gera um trio Pensamento → Ação (chamada de ferramenta) → Observação (retorno mockado). A calculadora usa um avaliador aritmético restrito (apenas números e operadores), então nada de código arbitrário é executado.

---

## Local Agent — ReAct Demo 🤖

A mini-agent that runs **100% in the browser**, with no LLM and no external calls. It takes a natural-language goal and simulates the **ReAct** loop (Reasoning + Acting): **Think → Act → Observe**, showing each step on a live timeline. The tools (`search`, `calculator`, `write_file`) are all mocked in JavaScript.

### ✨ Features

- Full ReAct loop visualized step by step (Thought, Action, Observation, Final answer)
- Three mocked tools: search, calculator (real, safe arithmetic evaluation) and file writing
- Planner that interprets the goal (detects numbers, search intent and write intent)
- Bilingual PT/EN interface with instant toggle
- Clickable examples to get started fast
- Single `index.html` file, no dependencies, no build step, no `localStorage`

### ▶️ How to use

1. Open `index.html` in any modern browser.
2. Type a goal (e.g., *"Calculate 15% of 240"*) or click an example.
3. Click **Run agent** and watch the agent's steps on the timeline.
4. Use the **PT / EN** button to switch language.

### 🧠 How it works

`planSteps(goal)` turns the goal into a ReAct script. Each detected intent produces a Thought → Action (tool call) → Observation (mocked return) triple. The calculator uses a restricted arithmetic evaluator (numbers and operators only), so no arbitrary code runs.

---

## 📄 License

MIT © 2026 Jonathan Ferreira Soares
