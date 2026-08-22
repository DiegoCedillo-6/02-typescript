# ⚡ Cheatsheet: De Java a TypeScript para Móviles
### Guía Rápida de Sintaxis, Comandos y Flujo de Entrega — 3° BGU Informática (UETS)

---

## 🍴 Flujo de Trabajo en 4 Pasos (Fork & Pull Request)

```bash
# PASO 1: En GitHub, haz clic en el botón 🍴 "Fork" (arriba a la derecha) en:
# https://github.com/UETS-Programacion-Movil/02-typescript

# PASO 2: Clona TU fork personal en tu computadora (reemplaza TU-USUARIO):
git clone https://github.com/TU-USUARIO/02-typescript.git
cd 02-typescript

# PASO 3: Crea tu rama de entrega con tu nombre y apellido:
git checkout -b entrega/mateo-vintimilla

# PASO 4: Instala dependencias y resuelve los retos en src/:
pnpm install
```

---

## 🛠️ Comandos de Prueba y Validación

```bash
# Probar cada reto individualmente mientras programas:
pnpm run start:01   # Reto 01: Tipos Primitivos
pnpm run start:02   # Reto 02: Interfaces y Puente Java
pnpm run start:03   # Reto 03: Estados Móviles y Uniones
pnpm run start:04   # Reto 04: Desafío Integrador Bar Salesiano

# Verificar que no tengas NINGÚN error de tipos (0 errores):
pnpm run check

# Ejecutar toda la suite completa:
pnpm run test:all
```

---

## 📤 Guardar, Subir y Entregar tu Tarea

```bash
# 1. Guarda tus cambios con Commits Semánticos (feat, fix, docs):
git add .
git commit -m "feat(reto-01): resolver tipos y promedios"

# 2. Sube tu rama a tu Fork en GitHub:
git push origin entrega/mateo-vintimilla

# 3. En GitHub Web: Entra a tu fork y haz clic en "Contribute" ➔ "Open pull request".
# Llena la plantilla y pega el link de tu video Screencast de 3 minutos.
```

---

## ☕ Java vs ⚡ TypeScript: Tabla Comparativa

| Concepto | ☕ Java (POO Clásica) | ⚡ TypeScript (Ecosistema Móvil) |
| :--- | :--- | :--- |
| **Enteros & Decimales** | `int a = 10; double b = 5.9;` | `const a: number = 10; const b: number = 5.9;` |
| **Cadenas de Texto** | `String nombre = "Juan";` | `const nombre: string = "Juan";` |
| **Booleanos** | `boolean activo = true;` | `const activo: boolean = true;` |
| **Arreglos** | `String[] lista = {"A", "B"};` | `const lista: string[] = ["A", "B"];` |
| **Colecciones** | `List<String> items = new ArrayList<>();` | `const items: Array<string> = [];` |
| **Constantes / Inmutabilidad** | `final int MAX = 100;` | `const MAX = 100;` o `readonly id: string;` |
| **Contrato de Datos** | `public class Alumno { ... getters/setters }` | `export interface Alumno { nombre: string; }` |
| **Valores Opcionales** | `Optional<String> tel;` | `telefono?: string;` |
| **Unión de Tipos** | Enums pesados o Interfaces heredadas | `type Estado = "cargando" \| "exito" \| "error";` |
| **Funciones / Métodos** | `public int sumar(int a, int b) { return a+b; }` | `export const sumar = (a: number, b: number): number => a + b;` |
| **Módulos** | `package com.uets.app; import ...` | `export { ... }; import { ... } from "...";` |

---

## 🛡️ Las 5 Reglas de Oro de TypeScript

1. **Usa `const` por defecto:** Usa `let` solo si la variable cambiará de valor; ¡jamás uses `var`!
2. **Cero `any`:** `any` apaga la seguridad de TypeScript. Si el dato es incierto de una API, usa `unknown` y valida con `typeof`.
3. **Propiedades Opcionales con `?`:** Si un dato puede no existir (ej. teléfono o foto), márcalo con `?` y accede con *Optional Chaining* (`usuario?.telefono`).
4. **Interfaces para Modelos, Types para Uniones:**
   - Usa `interface Usuario { ... }` para modelar objetos y entidades.
   - Usa `type Rol = "ADMIN" | "ESTUDIANTE"` para uniones y tipos literales.
5. **Tipa los retornos de las funciones:** Siempre indica qué devuelve una función: `(x: number): string => ...`.
