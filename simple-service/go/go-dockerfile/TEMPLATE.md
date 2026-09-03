# Go Service Dockerfile

Multi-stage Go Dockerfile + compose fragment + entrypoint: ./cmd/{{ .AgentName }}

## Scaffold

- **nodeKind:** `agent`
- **patternKind:** `simple-service`
- **techStack:** ['Go']
- **templatesApiVersion:** `1`

## Required TemplateContext

Use manifest `contextMapping` and file path placeholders (`{{ .AgentName }}`, etc.).

## Files

- `agents/{{ .AgentName }}/Dockerfile` ← `Dockerfile.tmpl`
- `agents/{{ .AgentName }}/docker-compose.fragment.yml` ← `docker-compose.fragment.yml.tmpl`
- `agents/{{ .AgentName }}/docker-compose.yml` ← `docker-compose.yml.tmpl`
- `cmd/{{ .AgentName }}/main.go` ← `main.go.tmpl`
