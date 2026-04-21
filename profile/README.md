# 🩺 Proyecto Sarah | Sarah-Health-AI

Bienvenido a la organización oficial de desarrollo de **Sarah**, el Agente de Inteligencia Artificial diseñado para el acompañamiento y seguimiento clínico de pacientes médicos.

## 🎯 Nuestra Misión
Centralizar, modernizar y escalar la experiencia del paciente y la gestión médica mediante tecnología de punta, asegurando un acompañamiento en tiempo real y el cumplimiento de la normativa de salud vigente.

---

## 👥 Estructura de Equipos

El desarrollo de Sarah está dividido en 5 frentes especializados:

* **`@team-ui-paciente`**: Interfaz de acompañamiento, chat interactivo y panel del paciente.
* **`@team-dashboard-medico`**: Visualización clínica y seguimiento de pacientes para el personal de salud.
* **`@team-gestion-medica`**: Herramientas administrativas e institucionales de la clínica.
* **`@team-backend`**: Lógica de negocio, APIs, base de datos y autenticación de usuarios.
* **`@team-ai-core`**: Desarrollo, entrenamiento e integración del Agente de Inteligencia Artificial (LLM).

---

## 🛠️ Estándar Tecnológico (Frontend)

Para mantener la coherencia visual y técnica en todas las interfaces del ecosistema Sarah, los equipos de UI y Dashboards operan bajo el siguiente stack acordado:

* **Core:** React + TypeScript + Vite + Tailwind CSS
* **Librería de Componentes:** [Base UI](https://base-ui.com/react/components) (Headless para control total del diseño).
* **Gráficos y Métricas:** [Recharts](https://recharts.org/)
* **Iconografía:** [Lucide React](https://lucide.dev/)
* **Animaciones:** [Motion](https://motion.dev/) (Uso sutil para retroalimentación del sistema y respuestas de la IA).
* **Tipografía:** Work Sans (Google Fonts)

---

## 🎨 Diseño y Sistema de Colores (Design System)

Toda la plataforma soporta Modo Claro y Modo Oscuro nativo a través de variables de CSS.

**Modo Claro (Por defecto):**
* **Fondo Principal:** `#f5f8fd` (Slate muy claro)
* **Fondo Secundario:** `#dfe2e8`
* **Texto Primario:** `#1f293b`
* **Texto Secundario:** `#67778c`
* **Accent (Primario):** `#0db17f` (Emerald)
* **Accent Hover:** `#17785a`

**Modo Oscuro:**
* **Fondo Principal:** `#1f273a`
* **Fondo Secundario:** `#1c2436`
* **Texto Primario:** `#f1f6fa`
* **Texto Secundario:** `#90a1b2`
* **Accent (Primario):** `#35b498`
* **Accent Hover:** `#12956c`

---

## 🚀 Flujo de Trabajo y Ramas (Branching)

Todos los repositorios dentro de esta organización deben seguir un flujo estricto para proteger los entornos de producción:

1. **Ramas de Funcionalidad (`feature/` o `bugfix/`):** Todo desarrollo nuevo debe hacerse en una rama derivada de `main`.
2. **Pull Requests (PR):** Para integrar código a `main`, se debe abrir un PR.
3. **Revisión de Código:** Todo PR debe ser aprobado por al menos **1 miembro distinto** al autor original antes de hacer *Merge*.
4. **Despliegue:** En la fase actual del proyecto, las interfaces se despliegan en Vercel para pruebas de QA. La infraestructura de producción final (On-Premise / Cloud de Salud) está en proceso de definición.

> *"Código limpio, tipado estricto y foco en la accesibilidad del paciente."*
