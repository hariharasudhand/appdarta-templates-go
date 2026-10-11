# Agent Runtime Overlay (Process, Native)

Local process launcher for runtime: process agents — go run entrypoint, PORT env, health hint. Docker-free app runtime (D1).

## Scaffold

- **nodeKind:** `agent`
- **patternKind:** `runtime-process`
- **techStack:** ['Go']
- **templatesApiVersion:** `1`

Preferred over `agent-runtime-process` for Go nodes packaged `runtime: process`
(resolveTemplateExtensions). Restored from appdarta d8650ea (D1 process runtime),
which P1-C4d deleted with config/code-templates before it reached the registry.

## Files

- `agents/{{ .AgentName }}/run-local.sh` ← `run-local.sh.tmpl`
