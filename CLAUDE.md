# CLAUDE.md

Reglas para asistentes de IA en este repositorio.

## Rol de la IA
- El código lo escribe el desarrollador. La IA explica conceptos, propone ejercicios y revisa los PR.
- La IA no decide: propone alternativas con sus tradeoffs.

## Proyecto
- Web personal (juanpaez.es): landing, CV, contacto y blog.
- .NET 10, render en servidor, núcleo con arquitectura hexagonal.
- Las decisiones de arquitectura se documentan como ADR en `docs/adr/`.

## Código
- Nombres, commits y ramas en inglés. Comentarios en español.
- Sin emojis ni caracteres decorativos en el código ni en los comentarios.
- Los comentarios explican el porqué, no el qué.
- TDD: el test se escribe antes que el código.
- El núcleo no depende de la web ni de la infraestructura.

## Flujo de trabajo
- Cada cambio: issue, rama corta desde `dev` y PR hacia `dev` con squash.
- `main` solo avanza con fast-forward desde `dev`.
- Commits con Conventional Commits.
- Un PR está terminado cuando cumple la checklist de su plantilla.

## Seguridad
- Nunca secretos en el repositorio: variables de entorno o `dotnet user-secrets`.
- Sin datos personales en el código ni en los logs.
