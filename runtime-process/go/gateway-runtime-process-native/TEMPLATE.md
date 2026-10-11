# Gateway Runtime Overlay (Process, Native)

Local process launcher for runtime: process gateway — go run entrypoint, GATEWAY_PORT/GATEWAY_CONFIG_DIR env, health hint. Docker-free app runtime (D1).

## Scaffold

- **nodeKind:** `gateway`
- **patternKind:** `runtime-process`
- **techStack:** ['Go']
- **templatesApiVersion:** `1`

Preferred over `gateway-runtime-process` for Go nodes packaged `runtime: process`
(resolveTemplateExtensions). Restored from appdarta d8650ea (D1 process runtime),
which P1-C4d deleted with config/code-templates before it reached the registry.

## Files

- `gateway/run-local.sh` ← `run-local.sh.tmpl`
