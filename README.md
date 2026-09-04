# Keycloak application stack for Kubernetes on Wodby

Deploy Keycloak applications on Kubernetes with Wodby.

This repository defines the Wodby stack manifests and default service
composition for Keycloak.

<!-- wodby:generated:start -->

## Stack contract

- [Keycloak stack on Wodby](https://wodby.com/stacks/keycloak)
- [Browse Wodby application stacks](https://wodby.com/stacks)
- [Wodby stack documentation](https://wodby.com/docs/2.0/stacks/)
- [Stack manifest reference](https://wodby.com/docs/2.0/stacks/template/)

## Service definitions

- [Keycloak service](https://github.com/wodby/service-keycloak)
- [PostgreSQL service](https://github.com/wodby/service-postgres)

## What's included

| Component / service | Default configuration |
| --- | --- |
| Keycloak<br>`keycloak` | required; enabled by default; links: `postgres` → `postgres` |
| PostgreSQL<br>`postgres` | required; enabled by default; volumes: `data` 20 GB |

Enabled optional services are selected by default but can be excluded when an
app is created. Disabled optional services are available but not selected by
default. Required services cannot be excluded.

## Validate the stack manifest

```bash
wodby stack validate-manifest stack.yml --org <org-id>
```

<!-- wodby:generated:end -->
