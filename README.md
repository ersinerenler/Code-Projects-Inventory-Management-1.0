# Code-Projects Inventory Management 1.0

Welcome to the Code-Projects Inventory Management 1.0 repository. This project aims to provide efficient inventory management.

## Security Vulnerabilities

### CVE-2023-46580

- **Description:** Stored Cross-Site Scripting (XSS) vulnerability via `editProduct.php`, 'pname' parameter.
- **Affected Version:** 1.0
- **Affected File:** `/Inventory-Management/model/editProduct.php`
- **Vulnerable Parameter:** 'pname'
- **Impact:** Attackers can inject and execute malicious scripts via the 'pname' parameter.
- **Solution:** Implement proper input validation and output encoding for the 'pname' parameter in `/Inventory-Management/model/editProduct.php`.

### CVE-2023-46581

- **Description:** SQL Injection vulnerability via `registration.php`, 'name', 'uname', and 'email' parameters.
- **Affected Version:** 1.0
- **Affected File:** `/Inventory-Management/view/registration.php`
- **Vulnerable Parameters:** 'name', 'uname', 'email'
- **Impact:** Attackers can manipulate SQL queries, potentially gaining unauthorized access or manipulating data.
- **Solution:** Implement parameterized queries and proper input validation for the affected parameters in `/Inventory-Management/view/registration.php`.

### CVE-2023-46582

- **Description:** SQL Injection vulnerability via `deleteProduct.php`, 'id' parameter.
- **Affected Version:** 1.0
- **Affected File:** `/Inventory-Management/model/deleteProduct.php`
- **Vulnerable Parameter:** 'id'
- **Impact:** Local attackers can execute arbitrary code by manipulating the 'id' parameter.
- **Solution:** Implement parameterized queries and proper input validation for the 'id' parameter in `/Inventory-Management/model/deleteProduct.php`.

---
