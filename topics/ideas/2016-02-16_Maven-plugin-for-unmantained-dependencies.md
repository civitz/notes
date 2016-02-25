---
title: maven plugin to check for unmantained dependencies
tags: [ java, maven, dependency, mantain, deprecated ]
type: text
---

# Service or maven plugin to check if dependencies are deprecated or unmantained.

## Possible ways without writing new code

### Maven enforcer plugin

[https://maven.apache.org/enforcer/enforcer-rules/bannedDependencies.html]()

Pro: we can push the conf in an institutional bom.xml 
Con: (un)authorized list must be mantained
Con: bom must be version-updated

Doubt: how does it handle transitive dependencies?
Doubt: how does it handle exceptions?

### OWASP dependency check

[https://www.owasp.org/index.php/OWASP_Dependency_Check](https://www.owasp.org/index.php/OWASP_Dependency_Check)

Based on CVE vulnerability database. Must check maven plugin capabilities.

Servizio/plugin maven: le librerie sono deprecate o non mantenute?

