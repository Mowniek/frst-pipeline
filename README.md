# frst-pipeline

Este proyecto implementa un flujo de trabajo automatizado utilizando GitHub Actions para validar la calidad del código mediante Integración Continua (CI).

## Estructura del Pipeline
* **Trigger:** Se activa automáticamente ante cualquier `push` en la rama `main`.
* **Entorno:** Servidor virtual con Ubuntu y Python 3.10.
* **Filtro de calidad:** Instala `flake8` y ejecuta un análisis estático (Linter) para detectar fallos de sintaxis antes de avanzar.

## Historial de Actions
En la pestaña de Actions se puede evidenciar el correcto funcionamiento del flujo:
1. Un fallo inicial provocado intencionalmente por un error de sintaxis en `script.py`, que mostro el pipeline en rojo.
2. La interpretación del log técnico y su subsecuente corrección, devolviendo el pipeline a estado verde.
