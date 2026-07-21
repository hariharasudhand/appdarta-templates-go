# REST Gateway

GW-* compliant gateway scaffold: mounts routes from handler YAMLs, real middleware

## Scaffold

- **nodeKind:** `gateway`
- **patternKind:** `rest-gateway`
- **techStack:** ['Go']
- **templatesApiVersion:** `1`

## Required TemplateContext

Use manifest `contextMapping` and file path placeholders (`{{ .AgentName }}`, etc.).

## Files

- `gateway/router.go` ← `router.go.tmpl`
- `gateway/middleware.go` ← `middleware.go.tmpl`
- `cmd/gateway/main.go` ← `main.go.tmpl`
- `gateway/Dockerfile` ← `Dockerfile.tmpl`
