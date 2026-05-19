# 🧪 Session 3 — AI for Testing

## 🎯 Goal
Use AI to assist in generating software test cases.

---

## 🧠 Scenario
A login feature needs comprehensive test coverage.

---

## 🧪 Prompt

### Initial Prompt
Generate test cases for a login page.

### Improved Prompt
You are a QA engineer.

Generate test cases for a login feature:
- Include valid and invalid scenarios
- Include edge cases

Return results in table format with:
- Test case ID
- Description
- Input
- Expected result

---

## 📊 Example Output

| ID | Description | Input | Expected Result |
|----|------------|------|----------------|
| TC01 | Valid login | correct credentials | Success |
| TC02 | Invalid login | incorrect password | Error message |
| TC03 | Empty fields | blank input | Validation error |

---

## 🧪 Additional Test Scenarios

- SQL injection attempts  
- Special characters  
- Long input values  
- Missing fields  

---

## 📊 Evaluation

| Criteria | Initial | Improved |
|----------|--------|---------|
| Structure | Poor | Strong |
| Usability | Low | High |
| Coverage | Limited | Expanded |

---

## 🔍 Observations

- AI can quickly generate diverse test cases  
- Structured prompts produce usable outputs  
- Outputs require validation by engineers  

---

## 🚀 Takeaway

AI can accelerate test design, but must be combined with domain expertise and validation.
