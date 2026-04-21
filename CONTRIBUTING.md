# Guía de Contribución y Buenas Prácticas 🛠️

¡Bienvenido al equipo de desarrollo del Proyecto Sarah! Para mantener la calidad, escalabilidad y legibilidad del código entre los 5 frentes de trabajo, todos los desarrolladores e ingenieros deben adherirse a las siguientes convenciones.

## 1. Estrategia de Ramas (Branching)
Nunca trabajamos directamente en `main`. Utilizamos un flujo basado en *Feature Branches*:
* `main`: Código en producción. Siempre estable y protegido.
* `feature/nombre-de-la-tarea`: Para nuevas funcionalidades (ej: `feature/login-cookies`).
* `bugfix/nombre-del-error`: Para arreglar errores (ej: `bugfix/crash-formulario-consentimiento`).
* `hotfix/error-critico`: Para errores urgentes en producción que no pueden esperar al ciclo normal.

## 2. Convención de Commits (Conventional Commits)
Los mensajes de commit deben ser descriptivos y seguir este formato estricto: `<tipo>: <descripción en minúsculas>`.

* `feat:` Nueva funcionalidad o característica.
* `fix:` Solución de un bug o error.
* `docs:` Cambios exclusivos en la documentación (README, comentarios).
* `style:` Cambios de formato (espacios, comas, punto y coma) que no afectan el código.
* `refactor:` Reescritura de código que no añade features ni arregla bugs (ej: optimización).
* `chore:` Tareas de mantenimiento (actualizar librerías, dependencias, Docker).

*Ejemplo correcto:* `feat: integra paleta de colores institucional en tailwind`

## 3. Estándares de Código
* **Tipado Estricto (TypeScript):** Prohibido el uso indiscriminado de `any`. Toda interfaz, prop o variable debe estar correctamente tipada.
* **Idioma:** El código (variables, funciones, componentes) puede estar en Inglés o Español, pero debe existir consistencia dentro del mismo módulo.
* **Comentarios:** Las explicaciones de lógica compleja o reglas de negocio de la clínica deben ir **siempre en Español**.

## 4. Flujo de Trabajo (Pull Requests)
1. Sube tu rama al repositorio remoto (`git push origin feature/tu-rama`).
2. Abre un *Pull Request (PR)* hacia la rama `main`.
3. En la descripción del PR, explica brevemente qué hace el código y si resuelve algún problema específico.
4. **Regla de Oro:** El PR debe ser revisado y aprobado por al menos **1 miembro distinto al autor original** del equipo correspondiente.
5. Una vez aprobado, y si los checks de compilación pasan correctamente, se realiza el *Merge*.
