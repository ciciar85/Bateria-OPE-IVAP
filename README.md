# 🏛️ Exámenes Oficiales IVAP — Cuerpo Administrativo C1 (Gobierno Vasco)

[![GitHub Pages](https://img.shields.io/badge/GitHub%20Pages-Desplegado-success?style=for-the-badge&logo=github)](https://ciciar85.github.io/Bateria-OPE-IVAP/)
[![Preguntas](https://img.shields.io/badge/Preguntas-373%20Oficiales-blue?style=for-the-badge)](preguntas.json)
[![Fundamentación Jurídica](https://img.shields.io/badge/Calibración-ivap--gestion--preguntas-emerald?style=for-the-badge)](#-fundamentación-jurídica-ivap-gestion-preguntas)
[![Convocatorias](https://img.shields.io/badge/Exámenes-2008%20|%202010%20|%202017%20|%202022-indigo?style=for-the-badge)](#-convocatorias-incluidas)
[![React](https://img.shields.io/badge/React%2018-SPA%20Autocontenida-61dafb?style=for-the-badge&logo=react)](index.html)

Web Test interactiva, simulador de examen y banco estructurado con las **373 preguntas oficiales reales** correspondientes a las cuatro convocatorias históricas de la **Escala de Administración General C1 (Cuerpo Administrativo)** del Gobierno Vasco: **Bolsa 2008**, **OPE 2010**, **Bolsa 2017** y **OPE 2022 (BEC 18/09/2022)**.

---

## ⚖️ Fundamentación Jurídica (`ivap-gestion-preguntas`)

Cada una de las 373 preguntas ha sido calibrada rigurosamente bajo el protocolo oficial `ivap-gestion-preguntas`:
- **Asignación a los 34 Temas Oficiales**: Cada pregunta cuenta con su asignación específica al temario vigente de la oposición C1.
- **Identificación de Norma y Artículo**: Cita concreta de la disposición legal de aplicación (Ley 39/2015, Ley 40/2015, Constitución Española, Ley 11/2022 de Empleo Público Vasco, TREBEP, Decreto Legislativo 1/2011 de Hacienda General de Euskadi, Ley 10/1982 del Euskera, Estatuto de Gernika, etc.).
- **Control de Obsolescencia y Reformas**: Marcado explícito de preguntas afectadas por derogación de normas anteriores (como la sustitución de la *Ley 30/1992* por la *Ley 39/2015*, de la *Ley 6/1989* por la *Ley 11/2022*, o de la *Ley 2/2004* por el *RGPD/LOPDGDD 3/2018*).
- **Justificación Técnico-Jurídica**: Literal del precepto legal que razona la opción correcta y desestima los distractores.

---

## 📋 Convocatorias Incluidas (373 Preguntas)

1. **Bolsa de Trabajo de Administrativos 2008**: 72 preguntas *(Bloque 1: Legislación y Temario General, Bloque 2: Procedimiento y Ofimática)*.
2. **Cuerpo Administrativo 2010**: 163 preguntas *(Bloques 1, 2, 3 y Caso Práctico oficial)*.
3. **Bolsa de Trabajo de Administrativos 2017**: 57 preguntas *(Bloque Único de examen)*.
4. **OPE 2022 (Examen BEC 18/09/2022)**: 81 preguntas *(Parte A: Temario General, Parte B Opción 1 y Parte B Opción 2)*.

---

## ⚡ Funcionalidades de la Web Test (`index.html`)

SPA construida en React 18 precompilado con Tailwind CSS. Carga de forma inmediata en cualquier dispositivo móvil o de escritorio:

1. 📖 **Modo Práctica / Estudio**:
   - Filtros desplegables por **Tema Oficial (1 al 34)**, **Convocatoria / Examen** (2008, 2010, 2017, 2022), **Bloques** y **Estado Normativo** (Vigentes vs Afectadas por Reforma).
   - Navegación ágil con botones o salto directo al número (1 a 373).
   - Atajos de teclado: flechas `←` / `→` para navegar y teclas `1`-`4` o letras `A`-`D` para contestar.
   - Panel de **Fundamentación Jurídica (ivap-gestion-preguntas)** con la norma, el artículo y el razonamiento legal.
   - Sistema de **Marcadores / Favoritos** persistente en `localStorage`.

2. ⏱️ **Modo Simulacro de Examen**:
   - Generación de exámenes aleatorios (50 preguntas) con cronómetro regresivo.
   - Corrección oficial del IVAP:
     $$\text{Puntuación} = \text{Aciertos} - \frac{\text{Fallos}}{3}$$
   - Pantalla de resultados con nota neta, porcentaje de acierto, apto/no superado y desglose completo.

3. 🔍 **Modo Explorador**:
   - Búsqueda en tiempo real por palabras clave, enunciado, opciones, artículos o convocatorias.

4. 📊 **Modo Estadísticas**:
   - Historial de progreso, aciertos, fallos, tasa de precisión y desglose por tema y examen.

5. 🌓 **Modo Oscuro / Claro**:
   - Interfaz conmutador dark/light para sesiones de estudio prolongadas.

---

## 📁 Estructura del Repositorio

- [`index.html`](index.html): Aplicación web completa y autónoma lista para GitHub Pages.
- [`preguntas.json`](preguntas.json): Dataset en JSON estructurado con las 373 preguntas, temas, estados y fundamentación jurídica.
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
