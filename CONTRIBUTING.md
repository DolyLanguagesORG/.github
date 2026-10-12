# Cómo contribuir

Gracias por sumarte a **DolyNation (Dolynglish)**. Esta es la guía por defecto
de la organización. La versión detallada vive en el repositorio de
documentación.

## Guías completas

- [Cómo hacer un Pull Request](https://github.com/DolyLanguagesORG/dolynation-ehecatl-docs/blob/develop/COMO-HACER-UN-PR.md) — flujo paso a paso, checks, `Closes #N`.
- [Flujo de trabajo](https://github.com/DolyLanguagesORG/dolynation-ehecatl-docs/blob/develop/FLUJO-DE-TRABAJO.md) — ramas, tablero, releases.
- [Convenciones](https://github.com/DolyLanguagesORG/dolynation-ehecatl-docs/tree/develop/conventions) — código, commits, API, testing.
- [Onboarding](https://github.com/DolyLanguagesORG/dolynation-ehecatl-docs/blob/develop/onboarding/setup.md) — cómo levantar el entorno.

## En cinco líneas

1. **Clona** el repo donde vas a trabajar:
   `git clone git@github.com:DolyLanguagesORG/<repo>.git`
2. **Instala** dependencias si las hay (`npm ci` en back y front).
3. **Levanta** el entorno local con el [onboarding](https://github.com/DolyLanguagesORG/dolynation-ehecatl-docs/blob/develop/onboarding/setup.md).
4. **Crea una rama desde `develop`**: `tipo/issue-<n>-<módulo>-<detalle>`
   (p. ej. `feat/issue-12-auth-login-page`). El número del issue es obligatorio.
5. **Abre un PR contra `develop`** siguiendo la guía y usando `Closes #<n>` en el
   cuerpo.

## Reglas que sí te bloquean

- El **título del PR** debe seguir **Conventional Commits** (lo valida el check
  `pr-title`).
- La **rama origen** debe respetar la convención y apuntar a `develop` (lo valida
  `pr-target`).
- El **merge** es exclusivamente **squash** y requiere que el CI pase.

## Reportar bugs o pedir features

Usa las plantillas de `.github/ISSUE_TEMPLATE/` de cada repositorio. Para
preguntas y dudas abiertas, usa las **Discussions** de la organización.
