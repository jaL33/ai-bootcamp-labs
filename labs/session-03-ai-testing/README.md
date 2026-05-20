# 🧪 Session 3 — AI for Testing

## 🎯 Goal
Use AI to assist in generating software test cases.

---

## 🧠 Scenario
A login feature needs comprehensive test coverage.

---

## 🎯 Key Pattern
Effective QA prompts typically include:
- Role definition (QA engineer)
- Clear output structure (table format)
- Coverage requirements (functional, edge, security)
- Explicit constraints

---

## 🧪 Prompt

### Initial Prompt
Generate test cases for a login page.

### Improved Prompt
You are a senior QA engineer.

Generate comprehensive test cases for a login feature.

Use a structured prompt with:
- Role definition
- Output format
- Coverage requirements

Cover:
- Functional scenarios
- Negative scenarios
- Boundary conditions
- Security risks (e.g. SQL injection, brute force attempts)

Return results in a table with:
- Test case ID
- Category (Functional / Negative / Security / Edge Case)
- Description
- Input
- Expected result

---

## 📊 Example Output

| ID | Category | Description | Input | Expected Result |
|----|----------|-------------|-------|-----------------|
| TC01 | Functional | Valid login | valid username + valid password | Authenticated and redirected to dashboard |
| TC02 | Negative | Invalid password | valid username + wrong password | Error shown: “Incorrect username or password” |
| TC03 | Edge Case | Empty fields | blank username + blank password | Validation errors for required fields |

---

## 📊 Evaluation

| Criteria | Initial | Improved |
|----------|--------|---------|
| Structure | Poor | Strong |
| Usability | Low | High |
| Coverage | Limited | Expanded |

---

## 📊 Output Comparison

| Prompt | Result |
|--------|--------|
| Basic | Generic, unstructured |
| Structured | Organised but limited coverage |
| QA-Oriented | Comprehensive, structured, and includes edge cases |

---

## 🔍 Observations

- AI can quickly generate diverse test cases  
- Structured prompts with role, format, and coverage guidance produce significantly more useful and complete test cases  
- Outputs require validation by engineers  

---

## 🚀 Takeaway

AI can accelerate test design, but must be combined with domain expertise and validation.
