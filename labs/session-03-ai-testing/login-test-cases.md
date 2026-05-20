# Login Feature Sample Test Cases

These sample test cases cover functional behavior, negative scenarios, boundary conditions, and security risks for a login feature.

| ID | Category | Description | Input | Expected result |
|----|----------|-------------|-------|-----------------|
| TC01 | Functional | Successful login with valid credentials | valid username + valid password | User authenticated and redirected to dashboard |
| TC02 | Functional | Successful login with remember-me enabled | valid username + valid password + remember-me selected | User authenticated and session persisted across browser restart |
| TC03 | Negative | Login fails with incorrect password | valid username + invalid password | Error shown: “Incorrect username or password” |
| TC04 | Negative | Login fails with unknown username | unknown username + valid password | Error shown: “Incorrect username or password” |
| TC05 | Negative | Login fails with empty username | blank username + valid password | Validation error: “Username is required” |
| TC06 | Negative | Login fails with empty password | valid username + blank password | Validation error: “Password is required” |
| TC07 | Edge Case | Login fails when both fields are empty | blank username + blank password | Validation error: “Username and password are required” |
| TC08 | Edge Case | Login rejects excessively long username | 256+ character username + valid password | Validation error or rejection; no crash |
| TC09 | Edge Case | Login rejects excessively long password | valid username + 256+ character password | Validation error or rejection; no crash |
| TC10 | Security | SQL injection attempt in username field | `admin' OR '1'='1` + any password | Login rejected; no unauthorized access |
| TC11 | Security | SQL injection attempt in password field | valid username + `password' OR '1'='1` | Login rejected; no unauthorized access |
| TC12 | Security | Script or special payload input | `"><script>alert(1)</script>` + any password | Input sanitized/rejected; no XSS or execution |
| TC13 | Security | Account lockout after repeated invalid attempts | valid username + wrong password repeated 5 times | Account locked or rate-limited; protective error displayed |
| TC14 | Edge Case | Username case sensitivity validation | valid username with wrong case + valid password | Login rejected if case-sensitive; no unintended success |
