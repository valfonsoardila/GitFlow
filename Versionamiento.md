# Guía de Git Flow

## Introducción a Git Flow
Git Flow es una estrategia de trabajo en Git que facilita la gestión de ramas y la implementación de nuevas funcionalidades, correcciones y despliegues. 

## Principales Ramas en Git Flow
1. **master**: Contiene el código en producción.
2. **develop**: Contiene el último código desarrollado y probado.

## Ramas Auxiliares
1. **feature/**: Se utilizan para desarrollar nuevas funcionalidades. Nacen de la rama `develop` y al finalizar se fusionan de nuevo en `develop`.
2. **release/**: Preparan el código para una nueva versión. Nacen de `develop` y se fusionan en `master` y `develop` una vez finalizadas.
3. **hotfix/**: Se utilizan para corregir errores críticos en producción. Nacen de `master` y se fusionan en `master` y `develop`.

## Comandos de Git Flow

### Iniciar Git Flow
Para iniciar Git Flow en tu proyecto:
```sh
git flow init