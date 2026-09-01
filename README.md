# Semana 02: Bases de TypeScript & Puente Pedagógico con Java ⚡📱
### Programación Móvil — 3° Bachillerato Técnico (2026–2027)

> [!INFO] Repositorio de Aprendizaje & Taller Práctico con Autograding
> **Institución:** Unidad Educativa Técnico Salesiano (UETS)  
> **Organización:** [UETS-Programacion-Movil](https://github.com/UETS-Programacion-Movil)  
> **Docente Elaborador:** Ing. Milton Velásquez  
> **Ponderación Evaluativa:** Metodología Dual MIT (50% Código en GitHub con Pull Request / 50% Video Screencast de 3 min)

---

## 🌟 Diapositivas Interactivas en Vivo (Cloudflare Workers)

Puedes acceder a la presentación interactiva proyectable (desarrollada con estética Neo-Brutalista y Lucide Icons) directamente desde la nube:

👉 **[Abrir Diapositivas en el Portal Oficial (Cloudflare Workers)](https://uets-pm-portal.vgmiltonisaac.workers.dev/02-typescript/)**

👉 **[Ver Portal Principal de la Materia](https://uets-pm-portal.vgmiltonisaac.workers.dev/)**

- ⌨ **Navegación:** Teclas `[←]` `[→]` o `[Espacio]`.
- 📺 **Pantalla Completa:** Presiona `[F]`.
- 🧠 **Quizzes Interactivos:** Evaluaciones formativas en vivo con retroalimentación instantánea.
- 💡 **Auto-Sync Test Runner:** Al ejecutar `pnpm test`, tus pruebas se sincronizan automáticamente con `main`.

---

## 🎯 ¿Qué tienes que hacer en este taller? (Paso a Paso)

El taller está compuesto por **4 Retos Prácticos**. En cada reto encontrarás un problema de desarrollo móvil, código con comentarios `// TODO:` para completar y un evaluador interactivo en terminal que te dirá en tiempo real si tus respuestas son correctas.

```text
🥊 Reto 01: Tipos Primitivos, Arrays y Fichas UETS (src/01_tipos_primitivos.ts)
🥊 Reto 02: De Clases Java POO a Interfaces TypeScript (src/02_puente_java_interfaces.ts)
🥊 Reto 03: Manejador de Estados Móviles & Uniones (src/03_unions_narrowing.ts)
🥊 Reto 04: Desafío Integrador — Carrito del Bar Salesiano (src/04_desafio_integrador.ts)
```

---

## 🚀 Guía de Git y Flujo de Trabajo para PrincipiANTES (Fork & Pull Request)

### Paso 1: Hacer Fork del Repositorio
1. En esta página de GitHub (arriba a la derecha), haz clic en el botón 🍴 **"Fork"**.
2. Selecciona tu cuenta personal y haz clic en **"Create fork"**. Ahora tendrás tu propia copia personal en GitHub.

### Paso 2: Clonar TU Fork en tu Computadora
Abre tu terminal en tu carpeta de proyectos y ejecuta (reemplaza `TU-USUARIO` por tu usuario de GitHub):
```bash
git clone https://github.com/TU-USUARIO/02-typescript.git
cd 02-typescript
```

### Paso 3: Instalar Dependencias
```bash
pnpm install
```

### Paso 4: Crear tu Rama de Trabajo Personal (¡NUNCA trabajes en `main`!)
Crea una rama con tu nombre y apellido:
```bash
# Ejemplo: si te llamas Mateo Vintimilla:
git checkout -b entrega/mateo-vintimilla
```

### Paso 5: Resolver los 4 Retos en VS Code
Abre los archivos en la carpeta `src/` y resuelve los bloques `// TODO:`. Puedes probar cada reto ejecutando:
```bash
# Probar el Reto 1:
pnpm run start:01

# Probar el Reto 2:
pnpm run start:02

# Probar el Reto 3:
pnpm run start:03

# Probar el Reto 4:
pnpm run start:04

# Probar TODOS los retos de una sola vez:
pnpm run test:all
```

### Paso 6: Verificar que no existan errores de compilación
Antes de subir tu tarea, corre:
```bash
pnpm run check
```
*(Debe terminar con 0 errores).*

### Paso 7: Guardar tus Cambios con Commits Semánticos
Usa mensajes claros siguiendo el estándar **Conventional Commits**:
```bash
git add .
git commit -m "feat(reto-01): tipar variables y calcular promedio"
git commit -m "feat(reto-02): traducir clase java a interface perfil"
git commit -m "feat(reto-03): implementar narrowing para estados de UI"
git commit -m "feat(reto-04): completar logica de carrito del bar salesiano"
```

### Paso 8: Subir tu Rama a TU Fork en GitHub
```bash
git push origin entrega/tu-nombre-apellido
```

### Paso 9: Abrir tu Pull Request (PR)
1. Entra a tu Fork en GitHub y haz clic en **"Contribute" ➔ "Open pull request"**.
2. Ponle de título: `Entrega Semana 2 - Tu Nombre y Apellido`.
3. En la descripción se cargará la plantilla oficial: escribe tu nombre, tu paralelo y el **enlace de tu video Screencast**.
4. Haz clic en **"Create pull request"**.
5. **🤖 ¡Mira la magia del Bot!** En menos de 1 minuto el bot de la UETS revisará tu código y comentará en tu PR tu calificación preliminar del **Bloque A (5.0 / 5.0 pts)**.

---

## 📹 Grabación del Screencast (Bloque B · 5.0 pts)

Graba un video de máximo **3:00 minutos** (usando [Loom.com](https://www.loom.com/), OBS o Clipchamp):
1. **0:00 - 0:30:** Muestra tu rostro en cámara y preséntate (Nombre y Paralelo).
2. **0:30 - 1:30:** Muestra tu editor VS Code y explica una de las `interfaces` que creaste y por qué usaste `readonly` o `?`.
3. **1:30 - 2:30:** Muestra tu terminal corriendo `pnpm run test:all` con todos los tests pasando en verde.
4. **2:30 - 3:00:** Explica en tus palabras una diferencia conceptual clave entre **Java** y **TypeScript** (ej. *Duck Typing* vs *Tipado Nominal*).

Pega el enlace público del video en la descripción de tu **Pull Request**.

---

## ⚖️ Rúbrica de Calificación Dual MIT (10.0 Puntos Total)

| Bloque Evaluativo | Criterio de Logro | Ponderación |
| :--- | :--- | :---: |
| **Bloque A: Pull Request en GitHub (50%)** | • 4 Retos completados y pasando tests (4.0 pts)<br>• Cero errores de tipos con `pnpm run check` (0.5 pts)<br>• Commits semánticos y Pull Request ordenado (0.5 pts) | **5.0 pts** |
| **Bloque B: Screencast Demostrativo (50%)** | • Justificación técnica del puente Java vs TypeScript (2.5 pts)<br>• Demostración en vivo en terminal con `tsx` (1.5 pts)<br>• Calidad de audio/video y enlace en PR (1.0 pt) | **5.0 pts** |
| **CALIFICACIÓN TOTAL** | **Suma Consolidada** | **10.0 pts** |

---

*Repositorio oficial de la Semana 02 — Módulo de Programación Móvil — Unidad Educativa Técnico Salesiano (UETS).*
