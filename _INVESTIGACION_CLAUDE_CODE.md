# 🔧 INVESTIGACIÓN: Cómo potenciar Claude Code para diseño web profesional

> Resumen de la investigación en GitHub, blogs técnicos y YouTube (mayo 2026) sobre las mejores herramientas para que Claude Code genere sitios profesionales con Stitch / Claude Design.

---

## 🎯 RESPUESTA CORTA

Lo que más impacto tiene es instalar **3 cosas**:

1. **Skill `awesome-design-md`** → 57 sistemas de diseño de marcas reales (Apple, Stripe, Airbnb, Notion, Anthropic) en formato markdown plug-and-play
2. **MCP `Playwright`** → Claude controla un navegador real (extrae sitios JS-renderizados, screenshots, scraping interactivo)
3. **MCP `Firecrawl`** → Scraping inteligente + extracción estructurada de cualquier sitio

Con estas 3, Claude Code investiga sitios mejor que un humano y diseña como un agency.

---

## 📦 REPOSITORIOS GITHUB CLAVE

### ⭐ Diseño visual (los más útiles para tu proyecto Hydrocell)

| Repo | Stars | Qué hace |
|---|---|---|
| **[VoltAgent/awesome-design-md](https://github.com/VoltAgent/awesome-design-md)** | 71K+ | 57 sistemas de diseño de marcas (Apple, Stripe, Notion, Anthropic, Uber...) en `.md` listos para usar. Le pasas uno a Claude y replica el estilo. |
| **[VoltAgent/awesome-claude-design](https://github.com/VoltAgent/awesome-claude-design)** | — | 68 inspiraciones de diseño en formato DESIGN.md específico para Claude |
| **[rohitg00/awesome-claude-design](https://github.com/rohitg00/awesome-claude-design)** | — | DESIGN.md por familia estética + recetas remix + skills + video teardowns |
| **UI/UX Pro Max** | — | Genera design system completo del proyecto. 67 estilos UI · 161 paletas · 57 combinaciones de fuentes |
| **Owl-Listener/designer-skills** | 833 | 63 skills + 27 comandos en 8 plugins cubriendo todo el ciclo de diseño |

### ⭐ Skills/Plugins generales

| Repo | Qué incluye |
|---|---|
| **[rohitg00/awesome-claude-code-toolkit](https://github.com/rohitg00/awesome-claude-code-toolkit)** | 135 agentes, 35 skills (+400K vía SkillKit), 42 comandos, 176 plugins, 20 hooks, 15 reglas, 7 templates, 14 MCP configs |
| **[ComposioHQ/awesome-claude-skills](https://github.com/ComposioHQ/awesome-claude-skills)** | Lista curada de Claude Skills |
| **[GetBindu/awesome-claude-code-and-skills](https://github.com/GetBindu/awesome-claude-code-and-skills)** | Colección de Claude Skills |
| **awesome-claude-code** | El catálogo principal de comandos, archivos y workflows |

### ⭐ MCPs

| Repo | Para qué |
|---|---|
| **[tolkonepiu/best-of-mcp-servers](https://github.com/tolkonepiu/best-of-mcp-servers)** | Lista ranqueada de MCPs, actualizada semanal |
| **awesome-mcp-servers** | Colección completa de MCPs por categoría |
| **MCP Servers Directory (Glama)** | Directorio web con búsqueda y filtros |

---

## 🔌 MCPs RECOMENDADOS PARA TU CASO (investigar + diseñar sitios)

### Para INVESTIGACIÓN web

```bash
# 1. Playwright MCP — navegador real (necesario para SPAs como Hydrocell originalmente)
claude mcp add playwright npx @playwright/mcp@latest

# 2. Firecrawl MCP — scraping inteligente con extracción estructurada
# Necesita API key: https://firecrawl.dev
claude mcp add firecrawl npx -y firecrawl-mcp \
  -e FIRECRAWL_API_KEY=tu_key_aqui

# 3. Brave Search MCP — búsquedas web sin Google
# Necesita API key: https://brave.com/search/api/
claude mcp add brave-search npx -y @modelcontextprotocol/server-brave-search \
  -e BRAVE_API_KEY=tu_key

# 4. GitHub MCP — clonar/explorar repos
claude mcp add github npx -y @modelcontextprotocol/server-github \
  -e GITHUB_PERSONAL_ACCESS_TOKEN=tu_token
```

### Para DISEÑO (lo que ya tienes + lo que falta)

```bash
# Stitch MCP — ya lo tienes ✅
# Vercel v0 MCP — alternativa a Stitch
# Figma MCP — si trabajas con Figma
claude mcp add figma npx -y figma-developer-mcp \
  -e FIGMA_API_KEY=tu_key
```

---

## 🎨 SKILLS PARA DISEÑO PROFESIONAL

### La oficial de Anthropic (277K+ installs)

```bash
# Frontend Design Skill — la oficial de Anthropic
# Genera "aesthetic choices, distinctive typography, purposeful color palettes,
#  and animations that feel intentional rather than decorative"
```

Para usarla: instala el plugin desde el marketplace oficial de Claude Code.

### Skills indispensables para tu caso

| Skill | Para qué |
|---|---|
| `frontend-design` | Aesthetic decisions, typography, color palettes |
| `awesome-design-md` | Replicar sistemas de marca conocidos |
| `ui-ux-pro-max` | Genera design system completo del proyecto |
| `designer-skills` (Owl-Listener) | 63 skills del ciclo completo |
| `tailwind-design-system` | Sistema con Tailwind |
| `accessibility-audit` | Auditar a11y |
| `design-handoff` | Generar package para developer |

---

## 📺 YOUTUBE — Tutoriales clave (mayo 2026)

| Video | Por qué verlo |
|---|---|
| **["Google Stitch 2.0 Tutorial: From Sketch to Code with Gemini 3.0"](https://www.youtube.com/watch?v=QGZ24YhbZT8)** | Stitch 2.0 acaba de salir, este tutorial es de referencia obligada |
| **["4 Ways to Make Beautiful Websites With Stitch 2.0"](https://www.youtube.com/watch?v=b0lwCDNOFUY)** | 4 técnicas distintas para sitios profesionales |
| **["Google Stitch + Google Antigravity Agents FREE Website tutorial"](https://www.youtube.com/watch?v=PYXewmzhunU)** | Cómo combinar Stitch con agentes para sitio completo |
| **["Google Stitch Tutorial for Beginners (Don't Waste Your Time)"](https://www.youtube.com/watch?v=COWMtnKjolM)** | Errores comunes y cómo evitarlos |
| **["How To Use Google Stitch: Easy Tutorial (2026)"](https://www.youtube.com/watch?v=3zTiND5f0_A)** | Tutorial completo desde cero |
| **["Awesome-design-md collection"](https://www.youtube.com/shorts/iGodxbTElCA)** | Explicación rápida del repo de design systems |

---

## ✨ MEJORES PRÁCTICAS PARA STITCH (consolidado de varios artículos)

### 1. Especificidad en el primer prompt
**❌ Mal:** "Diseña un dashboard"
**✅ Bien:** "Dashboard B2B de analytics con sidebar oscura, KPIs en cards arriba y tabla de datos abajo. Target: managers de mid-market. Paleta corporativa azul/blanco. Inspiración: Stripe Sessions."

### 2. Itera en fases (mirror professional designer)
- **Fase 1:** Layout y estructura solamente
- **Fase 2:** Colores y tipografía
- **Fase 3:** Spacing, microinteracciones, polish

### 3. Sube reference images
Subir un screenshot junto al prompt da estructura + dirección creativa. Combina screenshot del competidor con prompt: *"Usa este layout pero hazlo más moderno y minimalista"*.

### 4. Prompt refinement strategy
Cada vez que ajustas el prompt, Stitch regenera. Refina con vocabulario MUY específico (font names, hex codes, exact spacing).

### 5. Usa DESIGN.md como contexto
Antes de pedir el diseño, sube/incluye un `DESIGN.md` con:
- Brand identity
- Color palette (con hex)
- Typography scale
- Spacing system
- Components style
- Voice & tone

Resultado: Stitch sigue el sistema sin que tengas que repetirlo.

---

## 🚀 FLUJO RECOMENDADO PARA HYDROCELL

Basado en la investigación, **el setup óptimo para tu proyecto** sería:

### Paso 1: Instalar 3 MCPs claves
```bash
# Playwright para sitios JS-heavy
claude mcp add playwright npx @playwright/mcp@latest

# Firecrawl (con API key gratis)
claude mcp add firecrawl npx -y firecrawl-mcp -e FIRECRAWL_API_KEY=...

# GitHub para explorar repos
claude mcp add github npx -y @modelcontextprotocol/server-github -e GITHUB_PERSONAL_ACCESS_TOKEN=...
```

### Paso 2: Descargar el repo awesome-design-md
```bash
git clone https://github.com/VoltAgent/awesome-design-md.git ~/Documents/design-systems
```

### Paso 3: Para cada nuevo proyecto
1. Elegir un DESIGN.md de la colección (Apple, Stripe, etc.) o crear uno custom
2. Pegarlo en la raíz del proyecto
3. Usar Stitch con ese contexto: *"Crea homepage siguiendo este DESIGN.md"*
4. Iterar en fases (estructura → colores → polish)

### Paso 4: Investigación competitiva con Playwright
Cuando quieras analizar un sitio:
```
"Usa Playwright para abrir https://powerhho.com y dame todas sus secciones, paleta y tipografías"
```
Claude controlará un navegador real y extraerá info estructurada.

---

## 💡 CONCLUSIONES CLAVE

1. **El ecosistema MCP es enorme** — miles de servers disponibles en mayo 2026, no hay que usarlos todos
2. **`awesome-design-md` es el repo más útil** para replicar diseños profesionales (71K stars no mienten)
3. **Playwright MCP + Firecrawl** son la combinación killer para investigación web
4. **Stitch 2.0** acaba de salir con Gemini 3.0 — la calidad subió mucho
5. **El truco es DESIGN.md como contexto** — un solo archivo markdown bien hecho transforma la calidad del output

---

## 📚 RECURSOS DE LECTURA RECOMENDADOS

- **[Best MCP Servers for Claude Code 2026](https://www.truefoundry.com/blog/best-mcp-servers-for-claude-code)**
- **[50+ Best MCP Servers for Claude Code in 2026](https://claudefa.st/blog/tools/mcp-extensions/best-addons)**
- **[10 GitHub Repositories To Master Claude Code](https://www.kdnuggets.com/10-github-repositories-to-master-claude-code)**
- **[Best Claude Code Skills to Try in 2026](https://www.firecrawl.dev/blog/best-claude-code-skills)**
- **[The 18 Best Claude Code Skills for UI/UX Design](https://pasqualepillitteri.it/en/news/576/claude-code-skills-design-uiux-guide)**
- **[7 Claude Code Design Skills That Follow a Real Design Process](https://medium.com/@julian.oczkowski/7-claude-code-design-skills-that-follow-a-real-design-process-b871b8673d05)**
- **[Awesome Design MD: 4 Ways Builders Are Using It](https://www.mindstudio.ai/blog/awesome-design-md-71k-stars-4-ways-builders-claude-code)**
- **[Create Custom Brand DESIGN.md for Claude Code](https://www.mindstudio.ai/blog/custom-brand-design-md-claude-code-no-packages)**
- **[Claude Web Fetch vs Firecrawl](https://www.firecrawl.dev/blog/claude-web-fetch-vs-firecrawl)**
- **[Automate Browser Tasks with Claude Code and Playwright MCP](https://www.mindstudio.ai/blog/automate-browser-tasks-claude-code-playwright)**

---

## ⚡ ACCIONES INMEDIATAS QUE PODEMOS HACER

Si quieres, ahora mismo te configuro:

1. **Clonar awesome-design-md** localmente para usarlo como contexto
2. **Instalar Playwright MCP** (no requiere API key)
3. **Instalar Firecrawl MCP** (necesitas key gratuita de firecrawl.dev)
4. **Instalar GitHub MCP** (necesitas Personal Access Token)
5. **Generar un DESIGN.md custom de Hydrocell** consolidando todo lo que hemos diseñado

Dime cuál(es) quieres que ejecute.
