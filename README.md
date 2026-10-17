# 📣 Guía rápida: marketingskills — 40+ skills de marketing para tu agente (ES · PT)

Una sola página para usar **marketingskills** (de Corey Haines): qué es, cómo se instala, qué skill elegir para cada tarea de marketing y cómo empezar sin saber programar.

**Autor:** Guangyi Zhao · Octubre 2026

Proyecto original: https://github.com/coreyhaines31/marketingskills (55.202 estrellas, consultado el 17 de octubre de 2026)

> **Nota de autoría:** esta guía es una síntesis original, redactada por el autor a partir de la documentación pública del proyecto y de su propio uso. No es una traducción ni una copia de la documentación oficial, y no es un proyecto oficial de Corey Haines. Para el detalle completo, ve al repositorio enlazado.

---

## 🇪🇸 Español

### Qué es

marketingskills es una colección de más de 40 **skills** de marketing — archivos markdown que le dan a un agente de IA conocimiento especializado y flujos de trabajo para una tarea concreta. Cuando el agente detecta que estás trabajando en esa tarea, aplica los marcos y las buenas prácticas del skill correspondiente. Funciona con Claude Code, OpenAI Codex, Cursor, Windsurf y cualquier agente compatible con la especificación Agent Skills. Es gratuito y MIT, pensado para marketers técnicos y fundadores que quieren que el agente ayude con SEO, conversión, copy, anuncios y crecimiento.

### La pieza clave: product-marketing

Todos los skills leen primero **`product-marketing`**: ahí vive el contexto de tu producto, tu audiencia y tu posicionamiento. Es la base sobre la que trabaja el resto; sin ese contexto, cada skill parte de cero y los resultados suenan genéricos. Configúralo una vez, con calma.

### Instalación

```bash
# Todos los skills
npx skills add coreyhaines31/marketingskills

# Solo los que necesitas
npx skills add coreyhaines31/marketingskills --skill cro copywriting

# Ver la lista disponible
npx skills add coreyhaines31/marketingskills --list
```

La CLI detecta qué agentes tienes y dónde instalar (en Claude Code, `.claude/skills/`; los agentes universales comparten `.agents/skills/`). También se puede instalar como plugin de Claude Code desde su marketplace. Ojo: si lanzas el comando **desde dentro** de una sesión de Claude Code, puede instalar en el directorio universal que Claude Code no lee; pásale el agente explícito: `npx skills add coreyhaines31/marketingskills -a claude-code`.

### Qué skill para cada tarea

| Tarea | Skills |
|---|---|
| **SEO y descubrimiento** | `seo-audit` (auditoría técnica y on-page), `ai-seo` (aparecer en buscadores con IA), `programmatic-seo` (páginas a escala), `site-architecture` (jerarquía y URLs), `schema` (datos estructurados), `aso` (fichas de app stores) |
| **Conversión (CRO)** | `cro` (páginas y formularios), `signup` (registro), `onboarding` (activación), `popups`, `paywalls` |
| **Contenido y copy** | `copywriting` (copy de páginas), `copy-editing` (pulir textos), `cold-email` (prospección B2B), `emails` (flujos automáticos), `social`, `video`, `image`, `sms` |
| **Pagado y medición** | `ads` (Google, Meta, LinkedIn, X), `ad-creative` (creatividades a escala), `ab-testing` (experimentos), `analytics` (medición y auditoría de tracking) |
| **Crecimiento y retención** | `referrals` (referidos), `free-tools` (herramientas gratuitas como imán), `lead-magnets`, `churn-prevention` (cancelaciones y pagos fallidos), `community-marketing`, `co-marketing` |
| **Ventas y GTM** | `revops`, `sales-enablement`, `launch` (lanzamientos), `pricing` (precios y packaging), `prospecting`, `competitor-profiling` |
| **Estrategia** | `marketing-ideas` (ideas de crecimiento), `marketing-psychology` (modelos mentales), `customer-research` (investigar clientes), `competitors` (páginas comparativas) |

Los skills se cruzan entre sí: `copywriting` trabaja con `cro` y `ab-testing`; `customer-research` alimenta a `copywriting`, `cro` y `competitors`. No son comandos sueltos, son una red.

### Si no programas: tres pasos

1. **Instala un agente** con interfaz amable (Claude Code, Cursor o similar) y ábrelo en la carpeta de tu proyecto o negocio.
2. **Instala los skills** con el comando de arriba, empezando por `product-marketing` y rellenándolo con tu producto y tu cliente.
3. **Pide la tarea en lenguaje natural**: «audita el SEO de mi landing», «reescribe el titular pensando en este cliente». El agente elige el skill adecuado solo.

### ⚠️ Errores típicos

- **Saltarse product-marketing.** Es el error número uno: sin contexto de producto, el agente improvisa y todo suena a plantilla.
- **Instalar los 40+ de golpe sin necesitarlos.** Empieza por los de tu tarea de esta semana; el catálogo crece contigo.
- **Esperar datos que el agente no tiene.** Para auditar analytics o anuncios reales hay que conectarle las cuentas con el flujo guiado del proyecto (credenciales con alcance limitado, primer resultado en solo lectura).

---

## 🇵🇹 Português

### O que é

O marketingskills é uma coleção de mais de 40 **skills** de marketing — arquivos markdown que dão a um agente de IA conhecimento especializado e fluxos de trabalho para uma tarefa concreta. Quando o agente detecta que você está trabalhando naquela tarefa, aplica os frameworks e as boas práticas do skill correspondente. Funciona com Claude Code, OpenAI Codex, Cursor, Windsurf e qualquer agente compatível com a especificação Agent Skills. É gratuito e MIT, pensado para marketers técnicos e fundadores que querem que o agente ajude com SEO, conversão, copy, anúncios e crescimento.

### A peça-chave: product-marketing

Todos os skills leem primeiro o **`product-marketing`**: ali vive o contexto do seu produto, da sua audiência e do seu posicionamento. É a base sobre a qual o resto trabalha; sem esse contexto, cada skill parte do zero e os resultados soam genéricos. Configure uma vez, com calma.

### Instalação

```bash
# Todos os skills
npx skills add coreyhaines31/marketingskills

# Só os que você precisa
npx skills add coreyhaines31/marketingskills --skill cro copywriting

# Ver a lista disponível
npx skills add coreyhaines31/marketingskills --list
```

A CLI detecta quais agentes você tem e onde instalar (no Claude Code, `.claude/skills/`; os agentes universais compartilham `.agents/skills/`). Também dá para instalar como plugin do Claude Code pelo marketplace dele. Atenção: se você rodar o comando **de dentro** de uma sessão do Claude Code, ele pode instalar no diretório universal que o Claude Code não lê; passe o agente explícito: `npx skills add coreyhaines31/marketingskills -a claude-code`.

### Qual skill para cada tarefa

| Tarefa | Skills |
|---|---|
| **SEO e descoberta** | `seo-audit` (auditoria técnica e on-page), `ai-seo` (aparecer em buscadores com IA), `programmatic-seo` (páginas em escala), `site-architecture` (hierarquia e URLs), `schema` (dados estruturados), `aso` (páginas de app stores) |
| **Conversão (CRO)** | `cro` (páginas e formulários), `signup` (cadastro), `onboarding` (ativação), `popups`, `paywalls` |
| **Conteúdo e copy** | `copywriting` (copy de páginas), `copy-editing` (lapidar textos), `cold-email` (prospecção B2B), `emails` (fluxos automáticos), `social`, `video`, `image`, `sms` |
| **Pago e medição** | `ads` (Google, Meta, LinkedIn, X), `ad-creative` (criativos em escala), `ab-testing` (experimentos), `analytics` (medição e auditoria de tracking) |
| **Crescimento e retenção** | `referrals` (indicações), `free-tools` (ferramentas gratuitas como ímã), `lead-magnets`, `churn-prevention` (cancelamentos e pagamentos falhos), `community-marketing`, `co-marketing` |
| **Vendas e GTM** | `revops`, `sales-enablement`, `launch` (lançamentos), `pricing` (preços e packaging), `prospecting`, `competitor-profiling` |
| **Estratégia** | `marketing-ideas` (ideias de crescimento), `marketing-psychology` (modelos mentais), `customer-research` (pesquisar clientes), `competitors` (páginas comparativas) |

Os skills se cruzam entre si: `copywriting` trabalha com `cro` e `ab-testing`; `customer-research` alimenta `copywriting`, `cro` e `competitors`. Não são comandos soltos, são uma rede.

### Se você não programa: três passos

1. **Instale um agente** com interface amigável (Claude Code, Cursor ou similar) e abra na pasta do seu projeto ou negócio.
2. **Instale os skills** com o comando acima, começando pelo `product-marketing` e preenchendo com o seu produto e o seu cliente.
3. **Peça a tarefa em linguagem natural**: «audita o SEO da minha landing», «reescreve o título pensando neste cliente». O agente escolhe o skill adequado sozinho.

### ⚠️ Erros típicos

- **Pular o product-marketing.** É o erro número um: sem contexto de produto, o agente improvisa e tudo soa como modelo genérico.
- **Instalar os 40+ de uma vez sem precisar.** Comece pelos da sua tarefa desta semana; o catálogo cresce com você.
- **Esperar dados que o agente não tem.** Para auditar analytics ou anúncios reais é preciso conectar as contas com o fluxo guiado do projeto (credenciais com escopo limitado, primeiro resultado somente leitura).

---

## 🇬🇧 English summary

One-page cheat sheet (Spanish + Portuguese) for **marketingskills** (Corey Haines): the free, MIT-licensed collection of 40+ marketing skills — markdown files that give AI agents (Claude Code, Codex, Cursor, Windsurf, any Agent Skills-compatible agent) specialized frameworks for SEO, CRO, copywriting, ads, analytics and growth work. Covers installation with `npx skills add` (all skills, selected skills, or the plugin route, including the in-session `-a claude-code` gotcha), the foundation role of the `product-marketing` context skill that every other skill reads first, a task-to-skill table across seven categories (SEO & discovery, conversion, content & copy, paid & measurement, growth & retention, sales & GTM, strategy), the three-step path for non-programmers, and the typical mistakes: skipping the product context, installing everything at once, and expecting the agent to see account data it was never connected to. Original synthesis by the author from the project's public documentation; not an official document of the project and not a translation.

**Author:** Guangyi Zhao · October 2026 · MIT License
