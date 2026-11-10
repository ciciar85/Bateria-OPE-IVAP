# 🏛️ Exámenes Oficiales IVAP — Cuerpo Administrativo C1 (Gobierno Vasco)

[![GitHub Pages](https://img.shields.io/badge/GitHub%20Pages-Desplegado-success?style=for-the-badge&logo=github)](https://ciciar85.github.io/Bateria-OPE-IVAP/)
[![Preguntas](https://img.shields.io/badge/Preguntas-373%20Oficiales-blue?style=for-the-badge)](preguntas.json)
[![Convocatorias](https://img.shields.io/badge/Exámenes-2008%20|%202010%20|%202017%20|%202022-indigo?style=for-the-badge)](#-convocatorias-incluidas)
[![React](https://img.shields.io/badge/React%2018-SPA%20Autocontenida-61dafb?style=for-the-badge&logo=react)](index.html)

Simulador interactivo, web test y banco estructurado con las **373 preguntas oficiales reales** de los exámenes convocados por el **Instituto Vasco de Administración Pública (IVAP / HAEE)** para el **Cuerpo Administrativo (Escala de Administración General C1)**.

---

## 📋 Convocatorias Incluidas (373 Preguntas)

El banco oficial recopila los exámenes de las cuatro últimas convocatorias históricas del IVAP:

1. **Bolsa de Trabajo de Administrativos 2008**: 72 preguntas *(Bloque 1: Legislación y Temario General, Bloque 2: Procedimiento y Ofimática)*.
2. **Cuerpo Administrativo 2010**: 163 preguntas *(Bloques 1, 2, 3 y Caso Práctico oficial)*.
3. **Bolsa de Trabajo de Administrativos 2017**: 57 preguntas *(Bloque Único de examen)*.
4. **OPE 2022 (Examen BEC 18/09/2022)**: 81 preguntas *(Parte A: Temario General, Parte B Opción 1 y Parte B Opción 2)*.

---

## ⚡ Funcionalidades de la Web Test (`index.html`)

Single Page Application (SPA) construida en React 18 precompilado y estilizada con Tailwind CSS. Carga de forma ultra-rápida sin necesidad de servidor backend ni transpiladores lentos:

1. 📖 **Modo Práctica / Estudio**:
   - Selector directo por **Convocatoria** (2008, 2010, 2017, 2022) y por **Bloques de Examen**.
   - Navegación ágil pregunta a pregunta o salto directo al número (1 a 373).
   - Atajos de teclado para estudio rápido: flechas `←` / `→` para navegar, teclas numéricas `1`-`4` o letras `A`-`D` para contestar.
   - Retroalimentación inmediata con colores (verde acierto, rojo error).
   - Cita de plantilla oficial y literal de la solución.
   - Sistema de **Marcadores / Favoritos** persistente en `localStorage`.

2. ⏱️ **Modo Simulacro de Examen**:
   - Generación de exámenes aleatorios (50 preguntas) o completos.
   - Cronómetro regresivo oficial.
   - Corrección con la fórmula oficial del IVAP:
     $$\text{Puntuación} = \text{Aciertos} - \frac{\text{Fallos}}{3}$$
   - Pantalla de resultados con nota neta, porcentaje de acierto, apto/no superado y desglose completo.

3. 🔍 **Modo Explorador**:
   - Búsqueda en tiempo real por palabras clave, enunciado, opciones o convocatorias.

4. 📊 **Modo Estadísticas**:
   - Historial de progreso, aciertos, fallos, tasa de precisión y desglose por convocatoria con persistencia local.

5. 🌓 **Modo Oscuro / Claro**:
   - Interfaz conmutador dark/light para sesiones de estudio prolongadas.

---

## 📁 Estructura del Repositorio

- [`index.html`](index.html): Aplicación web completa y autónoma lista para GitHub Pages.
- [`preguntas.json`](preguntas.json): Dataset en JSON estructurado con las 373 preguntas, opciones y plantillas oficiales.
- [`Bateria_OPE_IVAP.md`](Bateria_OPE_IVAP.md): Documento íntegro en Markdown para consulta offline o impresión.
- [`.nojekyll`](.nojekyll): Deshabilita el procesado de Jekyll en GitHub Pages.
- [`README.md`](README.md): Documentación y guía del repositorio.

---

## 🚀 Despliegue en GitHub Pages

Para publicar o actualizar la Web Test:
1. En GitHub, dirígete a la pestaña **Settings** del repositorio `Bateria-OPE-IVAP`.
2. En la barra lateral izquierda, pulsa en **Pages**.
3. En **Build and deployment > Branch**, selecciona la rama `main` y la carpeta `/ (root)`.
4. Haz clic en **Save**. En unos instantes, la Web Test estará disponible en:
   ```
   https://ciciar85.github.io/Bateria-OPE-IVAP/
   ```
