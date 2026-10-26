# gentle-ai

## META
- id: gentle-ai
- owner: EduBalderas
- visibility: public
- idioma: en
- estado: estable
- tipo: producto
- nivel: L3
  - L0=gobernanza/política
  - L1=marca/metodología
  - L2=flujo/arquitectura
  - L3=producto ejecutable
  - L4=herramienta
- familia: gentle-ai
- origen: fork
- experimento: no
- nacido_de: Gentleman-Programming/gentle-ai
- orquestado_por: N/A
- brief_desde: N/A

## OBJETIVO
CLI en Go que configura el agente de IA que ya usas, con memoria Engram™, flujo ODD y revisión RDD.

## QUE_CONTIENE
- Binario `cmd/gentle-ai` (TUI Bubble Tea) y colector `cmd/gentle-telemetry`.
- 18 agentes en `internal/catalog/agents.go`: `claude-code`, `opencode`, `kilocode`, `gemini-cli`, `codex`, `cursor`, `vscode-copilot`, `antigravity`, `windsurf`, `kimi`, `qwen-code`, `kiro-ide`, `openclaw`, `pi`, `trae-ide`, `hermes`, `github-copilot-cli`, `conductor`.
- Componentes Engram, skills, Context7, persona, permissions, GGA y theme. CodeGraph es opt-in y queda fuera de los presets.
- Presets `full-gentleman`, `ecosystem-only`, `minimal` y `custom`.
- Flujo ODD, contrato RDD, `docs/`, `bench/`, `e2e/`, skills de contribuidor en `skills/` e instalador `scripts/install.sh`.
- Módulo `github.com/gentleman-programming/gentle-ai/v4`, Go 1.25.10, licencia MIT.

## CARACTERISTICAS
- Escribe la configuración nativa del agente ya instalado. Fórmula Homebrew: `gentleman-programming/tap/gentle-ai`.
- ODD deja el trabajo pequeño en línea. El trabajo sustancial crea `odd/tasks/<feature>.md` antes de editar código.
- Delega solo por exploración, escritores paralelos en superficies disjuntas, relevo de contexto o verificador independiente.
- Test-first cuando hay un test determinista y un resultado esperado.
- RDD arranca activo. `gentle-ai review mode disable` lo apaga y el candidato queda congelado antes de la lectura. Commit, push y release siguen en manos de quien usa el producto.
- RDD nativo en Claude Code, Codex, OpenCode y Pi. En Pi, Gentle Shell posee runtime, prompts y agentes.
- Copia la configuración antes de escribir. `gentle-ai doctor` solo lee.
- Conductor solo se detecta y no recibe archivos.
- macOS y Linux publican binarios de release. Windows se instala con `go install` y Go 1.25.10; el archivo oficial y Scoop siguen cerrados por Authenticode.

## FUERA_DE_ALCANCE
- Instalar el binario del agente.
- Runtime, prompts y ciclo de vida de Pi.
- Autorizar commit, push o release.
- Skills de framework: viven en Gentleman-Skills.
- Editor, shell y terminal: Gentleman.Dots es otra capa.
- Desinstalar CodeGraph.
- `gga init` por proyecto.
- Binarios y Scoop de Windows.
- SDD, retirado en v4.0.0.

## RELACIONES
- Upstream: https://github.com/Gentleman-Programming/gentle-ai
- Engram: https://github.com/Gentleman-Programming/engram
- Gentle Shell: https://github.com/Gentleman-Programming/gentle-shell
- Gentleman-Skills: https://github.com/Gentleman-Programming/Gentleman-Skills
- Gentleman.Dots: capa distinta, descrita en `docs/architecture.md`.
- Sitio: https://gentlemanprogramming.com/
- Wiki: https://gentle-ai-wiki.gentlemanprogramming.com/
- Marcas Gentle AI™ y Engram™ de Alan Buscaglia (`TRADEMARKS.md`). Esa nota cubre el resto del documento. Copyright del código: Gentleman Programming, MIT.
- Entrada: `docs/intended-usage.md`, `docs/quickstart.md`, `docs/agents.md`.

## ETIQUETAS
- cli
- go
- agentes
- odd
- rdd
- engram
- fork

## TOPICS_GITHUB
Este fork no publica topics. En el upstream `Gentleman-Programming/gentle-ai`:
- ai-coding
- claude-code
- code-review
- copilot
- cursor
- developer-tools
- golang
- llm
- mcp
- opencode
- persistent-memory
- spec-driven-development
- agent-skills
- ai-agents
- codex
- coding-agents
- pi
