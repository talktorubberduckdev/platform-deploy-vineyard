# Tenant Guide

⚠️ **This file is automatically managed by Crossplane. Do not edit manually.**

---

## 🏷 Tenant

`vineyard`

---

## 🌐 DNS

| Environment | Hostname |
|-------------|-----------|
| DEV  | `*.vny.dev.rezakara.demo` |
| TEST | `*.vny.test.rezakara.demo` |
| PROD | `*.vny.prod.rezakara.demo` |
| WL  | `*.vny.dev.rezakara.demo` |

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
