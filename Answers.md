# Answers to Part 3

Add your answers to the questions in Part 3, Step 2 below. 

## Vulernability Remediation:
### Vulnerability 1: 
1. Which package or library are you addressing?
pkg:pypi/pyyaml@5.1 or PyYAML

2. Which CVE is linked to this vulnerability?
CVE-2019-20477

3. What remediation steps do you suggest?
The issue for CVE-2019-20477, is centered around "insufficient restrictions on the load and load_all functions" (NIST, 2020). Because of these "insufficient restrictions" a malicious YAML can trigger arbitrary code execution. The reccomendation I would suggest, is to upgrade PyYAML to a safer version or avoiding the load/load_all functions.

### Vulnerability 2:
1. Which vulnerability are you addressing?
pkg:pypi/pillow@9.4.0 or the Python Imaging Library.

2. Which CVE is linked to this vulnerability?
CVE-2023-50447

3. What remediation steps do you suggest? 
CVE-2023-50447 also allows arbitrary code execution via "the environment parameter" (NIST, 2024). The best solution in this case would be to update the package. In the other CVE, we could limit the use of particular functions. In this CVE it would be immensely challenging to prevent an attacker from taking control of keys/names in the environment. 
