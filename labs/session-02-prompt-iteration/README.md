# 🔁 Session 2 — Prompt Iteration

This lab shows how prompt refinement can improve AI outputs through clearer instructions, role context, and format constraints.

## 🎯 Goal
Explore how different prompt variations affect response quality, consistency, and relevance.

---

## 🧠 Scenario
Multiple prompt versions are tested to identify the most effective way to ask the same question.

---

## 🧪 Prompts

### Prompt A
Explain API testing.

### Prompt B
Explain API testing using bullet points and include one example.

### Prompt C
You are a QA engineer.

Explain API testing to a beginner:
- Use simple language
- Provide 3 bullet points
- Include a real-world example
- Keep it under 120 words

---

## 📊 Example Output Comparison

| Prompt | Result |
|--------|--------|
| A | Unstructured explanation with minimal guidance |
| B | More structured, but still generic |
| C | Clear, concise, and tailored to the intended audience |

---

## 📊 Evaluation

| Criteria    | Prompt A | Prompt B | Prompt C |
|------------|----------|----------|----------|
| Clarity     | Low      | Medium   | High     |
| Structure   | Poor     | Medium   | Strong   |
| Relevance   | Low      | Medium   | High     |
| Consistency | Low      | Medium   | High     |

---

## 🧠 Key Insight

The most effective improvements were:

- Assigning a role (e.g. QA engineer)
- Defining clear output format (bullet points)
- Applying constraints (length, structure)

These changes consistently improved output quality and reliability across all responses.

---

## 🔁 Pattern Observed

The following prompt pattern consistently produced better results:

- Role + Audience
- Structured format (bullet points / tables)
- Explicit constraints (length, clarity)

This pattern can be reused across different AI tasks.

---

## 🚀 Takeaway

Small prompt improvements can transform AI output from vague and inconsistent into clear, structured, and relevant guidance.
