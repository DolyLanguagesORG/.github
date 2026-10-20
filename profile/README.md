# DolyNation

Plataforma web de **aprendizaje de idiomas con inteligencia artificial**:
genera lecturas adaptadas al nivel del usuario, evalúa la comprensión mediante
resúmenes calificados por procesamiento de lenguaje natural y analiza el
vocabulario en contexto con audio.

Idiomas iniciales: **inglés, francés, español e italiano**.

Proyecto académico del equipo de Desarrollo Web (septiembre–diciembre 2026).

> «Dolynglish» es el nombre histórico del proyecto; la documentación, el
> código y la entrega usan **DolyNation**.

## Repositorios

| Repo | Contenido | Stack |
| --- | --- | --- |
| [`dolynation-atl-back`](https://github.com/DolyLanguagesORG/dolynation-atl-back) | API REST | NestJS 11 · Drizzle · PostgreSQL |
| [`dolynation-tonatiuh-front`](https://github.com/DolyLanguagesORG/dolynation-tonatiuh-front) | Frontend web | Next.js 16 · TypeScript |
| [`dolynation-tlalli-infra`](https://github.com/DolyLanguagesORG/dolynation-tlalli-infra) | Infraestructura, Docker Compose y esquema SQL | Docker · PostgreSQL |
| [`dolynation-ehecatl-docs`](https://github.com/DolyLanguagesORG/dolynation-ehecatl-docs) | **Documentación, convenciones y anteproyecto** | Markdown |
| [`doly-languages`](https://github.com/DolyLanguagesORG/doly-languages) | Monorepo original — **archivado, sin uso**. La documentación vigente está en `dolynation-ehecatl-docs` | — |

## Documentación

Todo el material del proyecto vive en
**[`dolynation-ehecatl-docs`](https://github.com/DolyLanguagesORG/dolynation-ehecatl-docs)**:

| Documento | Para qué sirve |
| --- | --- |
| [Anteproyecto](https://github.com/DolyLanguagesORG/dolynation-ehecatl-docs/blob/develop/anteproyecto/anteproyecto-dolynation.md) | El proyecto académico: problema, alcance, MVP, requerimientos, riesgos, roles y cronograma |
| [Cronograma](https://github.com/DolyLanguagesORG/dolynation-ehecatl-docs/blob/develop/plan/cronograma.md) | Los 5 sprints, sus fechas, responsables y entregables |
| [Convenciones](https://github.com/DolyLanguagesORG/dolynation-ehecatl-docs/blob/develop/conventions/README.md) | Ramas, commits, contrato de la API, base de datos, seguridad y versionado |
| [Onboarding](https://github.com/DolyLanguagesORG/dolynation-ehecatl-docs/blob/develop/onboarding/setup.md) | Levantar el entorno (local o en Codespaces) |
| [Flujo de trabajo](https://github.com/DolyLanguagesORG/dolynation-ehecatl-docs/blob/develop/operations/FLUJO-DE-TRABAJO.md) | Ramas, tablero, CODEOWNERS, revisiones y releases |
| [Plan de despliegue](https://github.com/DolyLanguagesORG/dolynation-ehecatl-docs/blob/develop/operations/PLAN-DE-DESPLIEGUE.md) | Los 3 entornos, puertos, secretos y flujo de despliegue |
| [Justificación de GitHub](https://github.com/DolyLanguagesORG/dolynation-ehecatl-docs/blob/develop/operations/JUSTIFICACION-GITHUB.md) | Por qué GitHub es la plataforma principal de trabajo del proyecto |

## Cómo empezar

1. Lee la **[guía de contribución](https://github.com/DolyLanguagesORG/dolynation-ehecatl-docs/blob/develop/CONTRIBUTING.md)**.
2. Sigue el **[onboarding](https://github.com/DolyLanguagesORG/dolynation-ehecatl-docs/blob/develop/onboarding/setup.md)** para levantar el entorno.
3. Aprende el **[flujo de trabajo](https://github.com/DolyLanguagesORG/dolynation-ehecatl-docs/blob/develop/operations/FLUJO-DE-TRABAJO.md)**: ramas, tablero y releases.
4. Mira el **[cronograma](https://github.com/DolyLanguagesORG/dolynation-ehecatl-docs/blob/develop/plan/cronograma.md)** para saber qué toca y cuándo.

## Cómo trabajamos

- Ramas desde `develop`: `tipo/issue-<n>-<módulo>-<detalle>` (p. ej. `feat/issue-12-auth-login-page`).
- PRs siempre hacia `develop` con **squash**; `main` es solo releases y hotfixes.
- Mensajes de commit en **Conventional Commits**.
- CI obligatorio (lint, tests, build) y checks `pr-title` / `pr-target` / `pr-labels` antes de mergear.
- Cada PR necesita **1 aprobación de un code owner** (2 en `main`) y todos sus comentarios resueltos.
- Un issue por tarea, con entregables, criterios de aceptación y evidencia.

## Equipo

Los roles y responsabilidades son los del §11.2 del
[anteproyyecto](https://github.com/DolyLanguagesORG/dolynation-ehecatl-docs/blob/develop/anteproyecto/anteproyecto-dolynation.md).

| Cuenta | Persona | Rol | De qué se encarga | Repos donde es code owner |
| --- | --- | --- | --- | --- |
| [@XxjesusalbertoxX](https://github.com/XxjesusalbertoxX) | Jesús Alberto Villarreal Pérez | **Scrum Master / Lead Developer** | Coordinación del flujo en GitHub, CI/CD, revisión de PRs, releases e infraestructura | `atl-back`, `tlalli-infra`, `tonatiuh-front`, `ehecatl-docs` |
| [@SebastianRdzC04](https://github.com/SebastianRdzC04) | Sebastián Rodríguez Contreras | **Product Owner** | Prioriza el backlog, valida los criterios de aceptación y aprueba el cierre de cada issue | `ehecatl-docs` |
| [@AzaelG26](https://github.com/AzaelG26) | Aozmar Azael García Candela | **Desarrollador Backend (principal)** | Módulos del backend, autenticación criptográfica, conector con la IA y motor de evaluación | `atl-back`, `tlalli-infra` |
| [@EliasGalarza333](https://github.com/EliasGalarza333) | José Elías Galarza Pedroza | **Desarrollador Backend (soporte)** | DTOs, endpoints de perfil, historial, módulo administrativo y QA de integración | `atl-back`, `tlalli-infra` |
| [@y0ADQ1](https://github.com/y0ADQ1) | Juan Antonio Deras Durón | **Desarrollador Frontend** | Maquetado responsivo, visor de lectura, pop-up contextual y dashboard | `tonatiuh-front`, `ehecatl-docs` |

Además, [`@JesusDelToroRobledoUTT`](https://github.com/JesusDelToroRobledoUTT)
tiene acceso de solo lectura como asesor del proyecto.

> **Para aparecer en la pestaña *People* de la organización**, cada integrante
> tiene que activar su perfil público desde su propia cuenta: *Settings →
> Public profile → Make this organization public*. GitHub no permite que otro
> lo haga por ellos.

> Los repos llevan nombres de deidades nahuas: **Atl** (agua), **Tonatiuh**
> (sol), **Tlalli** (tierra) y **Ehecatl** (viento).
