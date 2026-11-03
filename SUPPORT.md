# Tenant Guide

⚠️ **This file is automatically managed by Crossplane. Do not edit manually.**

---

## 🏷 Tenant

`vineyard`

---

## 🌐 DNS

| Environment | Hostname |
|-------------|-----------|
| DEV  | `*.vineyard.dev.rezakara.demo` |
| TEST | `*.vineyard.test.rezakara.demo` |
| PROD | `*.vineyard.prod.rezakara.demo` |
| WL  | `*.vineyard.dev.rezakara.demo` |

---

## 🚦 HTTPRoute / Gateway

```yaml
parentRefs:
  - group: gateway.networking.k8s.io
    kind: Gateway
    name: "vineyard"
    namespace: platform-system
    sectionName: https
```

---
