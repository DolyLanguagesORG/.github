# DolyNation · repositorio de organización `.github`

Este repositorio **no contiene código de producto**. Guarda los **archivos
por defecto de la organización** [DolyLanguagesORG](https://github.com/DolyLanguagesORG)
y la **portada** que GitHub muestra en la página de la organización.

## Qué hay aquí

| Ruta | Para qué sirve |
| --- | --- |
| [`profile/README.md`](./profile/README.md) | Portada pública de la organización (`github.com/DolyLanguagesORG`). |
| [`CONTRIBUTING.md`](./CONTRIBUTING.md) | Guía de contribución por defecto, para los repos que no tengan la suya. |
| [`CODE_OF_CONDUCT.md`](./CODE_OF_CONDUCT.md) | Código de conducta por defecto para todos los repos. |
| [`SECURITY.md`](./SECURITY.md) | Política de reporte de vulnerabilidades por defecto. |
| [`SUPPORT.md`](./SUPPORT.md) | Canales de soporte por defecto. |

## Por qué existe

GitHub le da un trato especial a un repositorio público llamado `.github`
dentro de una organización:

- Los **archivos comunitarios** que pongas aquí se usan en **cualquier repo de
  la organización que no tenga el suyo propio**. Así no hay que copiarlos en
  cada repo.
- El archivo `profile/README.md` se muestra como **portada** en la página de la
  organización.

El código del proyecto vive en los repos de trabajo:

- [`dolynation-atl-back`](https://github.com/DolyLanguagesORG/dolynation-atl-back) — API REST (NestJS)
- [`dolynation-tonatiuh-front`](https://github.com/DolyLanguagesORG/dolynation-tonatiuh-front) — Frontend (Next.js)
- [`dolynation-tlalli-infra`](https://github.com/DolyLanguagesORG/dolynation-tlalli-infra) — Infraestructura / Docker Compose
- [`dolynation-ehecatl-docs`](https://github.com/DolyLanguagesORG/dolynation-ehecatl-docs) — **Documentación, convenciones y anteproyecto**

Y [`doly-languages`](https://github.com/DolyLanguagesORG/doly-languages) — el
monorepo original, **archivado y sin uso**: la documentación vigente vive en
`dolynation-ehecatl-docs`.

## Notas

- Este repo debe ser **público**: GitHub solo aplica los archivos por defecto
  desde un repo `.github` público.
- Los repos que ya tienen su propio `PULL_REQUEST_TEMPLATE.md`,
  `ISSUE_TEMPLATE/` o `CONTRIBUTING.md` **conservan los suyos**; los de aquí
  solo actúan como respaldo.
- Aquí **no** viven workflows reutilizables: mover un job a un workflow
  reutilizable renombra su check (`<job-caller> / <job-callado>`) y rompería
  los *required status checks* de los rulesets. El CI de validación se queda en
  cada repo.
