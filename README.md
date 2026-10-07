# Calidad de Software

Repositorio de apoyo para la materia **Calidad de Software**. Reúne conceptos básicos y orientaciones para aplicar prácticas de calidad en proyectos web con **HTML, CSS, JavaScript, ReactJS y NestJS**.

## ¿Qué es la calidad de software?

Es el grado en que un sistema cumple los requisitos y satisface las necesidades de sus usuarios. También considera características como:

- **Funcionalidad:** ofrece las funciones esperadas.
- **Usabilidad:** resulta fácil de aprender y utilizar.
- **Confiabilidad:** funciona de manera correcta y consistente.
- **Eficiencia:** aprovecha adecuadamente el tiempo y los recursos.
- **Mantenibilidad:** puede corregirse y evolucionar con facilidad.
- **Seguridad:** protege los datos y controla el acceso.

## Aseguramiento y control de calidad

- **Aseguramiento de calidad (QA):** actividades preventivas que mejoran el proceso de desarrollo; por ejemplo, definir estándares y revisar código.
- **Control de calidad (QC):** actividades para detectar defectos en el producto; por ejemplo, ejecutar pruebas y verificar resultados.

## Pruebas de software

Las pruebas ayudan a encontrar defectos y comprobar que el sistema se comporta según lo esperado. Un buen caso de prueba define entradas, condiciones y el resultado esperado. Las pruebas complementan otras prácticas de calidad, pero no pueden demostrar por sí solas que un programa esté libre de defectos.

### Pruebas unitarias

Verifican una unidad pequeña de código —como una función, método o componente— de forma aislada. Suelen ser rápidas y ayudan a localizar con precisión los errores. Las dependencias externas pueden reemplazarse por mocks o stubs.

**Ejemplo:** comprobar que una función que calcula un total aplique correctamente un descuento.

En proyectos JavaScript/TypeScript se pueden usar herramientas como **Jest** o **Vitest**.

### Pruebas de integración

Comprueban que varias unidades o componentes colaboren correctamente, por ejemplo, un servicio junto con una base de datos o una API.

### Pruebas E2E (End-to-End)

Validan un flujo completo desde la perspectiva del usuario, recorriendo las partes principales de la aplicación. Por ejemplo: iniciar sesión, buscar un producto y completar una compra. Son útiles para detectar problemas de integración, aunque suelen ser más lentas y requieren más preparación que las pruebas unitarias.

Herramientas habituales para aplicaciones web: **Playwright** y **Cypress**.

## Pirámide de pruebas

Como orientación general, conviene tener muchas pruebas unitarias, una cantidad moderada de pruebas de integración y un conjunto más pequeño de pruebas E2E para los flujos críticos.

## Buenas prácticas

1. Diseñar pruebas con resultados esperados claros y verificables.
2. Probar casos normales, límites y entradas inválidas.
3. Mantener las pruebas independientes, legibles y repetibles.
4. Ejecutar las pruebas después de cada cambio y corregir los fallos.
5. No confundir cobertura de código con calidad: cubrir una línea no garantiza que su comportamiento esté bien verificado.
6. Evitar incluir credenciales o datos sensibles en el repositorio.

## Herramientas y ejecución

Este repositorio está preparado para alojar proyectos del ecosistema Node.js; el archivo `.gitignore` excluye dependencias, variables de entorno, artefactos de compilación y reportes de pruebas. Los comandos disponibles dependen de cada proyecto y de sus scripts configurados en `package.json`. Como ejemplos, los proyectos suelen definir scripts para ejecutar pruebas unitarias y pruebas E2E mediante su herramienta correspondiente.

## Objetivo del repositorio

Utilizar conceptos y herramientas de calidad de software para planificar, desarrollar y verificar aplicaciones mantenibles, confiables y centradas en las necesidades de sus usuarios.
