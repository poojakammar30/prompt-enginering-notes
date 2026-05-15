Markdown
# Prompt Engineering: Unlocking LLM Potential

[cite_start]Prompt engineering is essentially **programming in natural language**[cite: 17, 254]. [cite_start]Instead of using code, you provide instructions in plain language to define a model's task, role, and constraints[cite: 18, 19]. [cite_start]Because LLMs function through **next-token prediction**, the context and structure you provide directly shape the relevance of the output[cite: 33, 36, 38].

---

## Core Prompting Techniques

### 1. Specificity & Scene Setting
[cite_start]Define clear parameters so the model doesn't have to guess[cite: 49]. 
* [cite_start]**Role:** Assign a persona (e.g., "Senior B2B Copywriter")[cite: 10, 50].
* [cite_start]**Audience:** Specify who the content is for (e.g., "ops managers")[cite: 11, 51].
* [cite_start]**Tone:** Describe the style (e.g., "confident but not salesy")[cite: 11, 52].
* [cite_start]**Format:** Dictate the structure (e.g., "numbered steps")[cite: 53].

### 2. Few-Shot Prompting
[cite_start]Provide **2–4 examples** of input-output pairs[cite: 65]. [cite_start]This allows the model to infer patterns, which is particularly useful for formatting, styling, or classification tasks[cite: 65, 66].

### 3. Chain-of-Thought (CoT)
[cite_start]Ask the model to **reason step-by-step** before providing a final answer[cite: 81]. [cite_start]This technique reduces errors in logic, math, and multi-step planning[cite: 82].
> [cite_start]**Example:** "Think step by step: find the subtotal, apply the discount, then state the final amount"[cite: 94].

### 4. Structured Output
[cite_start]Request specific machine-readable or organized formats like **JSON, tables, or Markdown** to make the output easier to parse or use in other applications[cite: 97, 98].

### 5. Interview-Style Prompting
[cite_start]For complex tasks, ask the model to **interview you**[cite: 141, 142]. 
1. [cite_start]State your goal[cite: 147].
2. [cite_start]Instruct the model to ask clarifying questions one at a time[cite: 151].
3. [cite_start]Provide answers until the model has enough context to perform the task accurately[cite: 151, 153].

---

## Comparison: Steering vs. Commanding

| Feature | Commanding (Weak) | Steering (Strong) |
| :--- | :--- | :--- |
| **Approach** | [cite_start]Simple, vague instruction[cite: 41]. | [cite_start]Detailed role, audience, and constraints[cite: 42, 46]. |
| **Example** | [cite_start]"Write an email"[cite: 45]. | [cite_start]"You are replying to a client... Propose a new deadline: March 15. Tone: professional"[cite: 45]. |
| **Result** | [cite_start]Generic, wrong tone or length[cite: 8, 202]. | [cite_start]Consistent, on-brand, and actionable[cite: 13, 20, 46]. |

---

## Advanced Strategies & Best Practices
* [cite_start]**Iterative Refinement:** Treat prompting as a conversation; refine the output by asking for specific changes (e.g., "Shorter," "More formal")[cite: 131, 132].
* [cite_start]**Prompt Chaining:** Break complex tasks into smaller steps where the output of one step becomes the input for the next[cite: 180, 181].
* [cite_start]**Temperature Control:** Use **low temperature** (e.g., 0.2) for factual/structured tasks and **higher temperature** (e.g., 0.8) for creative brainstorming[cite: 197, 198, 199].
* [cite_start]**Negative Constraints:** Explicitly state what to avoid (e.g., "No emojis," "Do not use jargon") to prevent off-topic tangents[cite: 12, 112, 115].
* [cite_start]**System vs. User Prompts:** Use **System Prompts** to set permanent rules and **User Prompts** for the specific task at hand[cite: 171, 172].
