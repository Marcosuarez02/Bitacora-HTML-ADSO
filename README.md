# Proyecto Formativo: Bitácora Web Semántica y Accesible en HTML Puro
**CENTRO INDUSTRIAL DE MANTENIMIENTO INTEGRAL (CIMI) - SENA**  
**Programa:** Tecnología en Análisis y Desarrollo de Software (ADSO)  
**Ficha:** 3381732 | **Competencia:** Desarrollo de Software  
**Aprendiz Autor:** Marco Antonio Suárez González  
**Equipo de Trabajo Colaborativo:** 
- **Marco Antonio Suárez González** (Líder Técnico - Vista 1: `index.html`)
- **Andrés Felipe Parra Aguilar** (Analista - Vista 2: `reglas.html`)
- **Miguel Serrano Díaz** (Auditor de Calidad - Vista 3: `trazabilidad.html`)  
**Guía:** GFPI-F-135 V04 - Momento 4: Transferencia del Conocimiento  

---

## 1. Descripción del Proyecto
Este proyecto transforma la bitácora estática de seguimiento desarrollada en Excel en una solución web profesional, interactiva, accesible y estructurada exclusivamente con **HTML puro (HTML5 semántico sin hojas de estilo CSS)**.

El sitio representa fielmente la estructura de los tres libros/hojas de la bitácora técnica institucional mediante tres vistas independientes e interconectadas a través de un panel de navegación superior.

---

## 2. Estructura de las Tres Vistas Independientes y Distribución

1. **`index.html` (Vista 1 - Información General) - *Desarrollado por Marco Antonio Suárez*:**
   - Muestra la ficha técnica institucional del proyecto: Programa, Competencia, Ficha 3381732, datos del aprendiz autor y equipo colaborativo.
   - Implementa cuadrícula nativa con `<table>`, `<thead>`, `<tbody>` y encabezados `scope="row"` / `scope="col"`.
2. **`reglas.html` (Vista 2 - Reglas y Lineamientos Técnicos) - *Desarrollado por Andrés Felipe Parra*:**
   - Expone los 4 principios de calidad de la bitácora: Responsabilidad Única (SRP), Cero Adjetivos Subjetivos, Inmutabilidad Histórica y Trazabilidad de Impedimentos.
   - Detalla la matriz técnica con el formato de las 7 columnas oficiales del formato SENA.
3. **`trazabilidad.html` (Vista 3 - Tabla de Trazabilidad Diaria) - *Desarrollado por Miguel Serrano*:**
   - Cuadrícula completa con la totalidad de registros técnicos de las actividades ejecutadas en Octubre de 2026.
   - Contiene los 12 registros correspondientes a las semanas 2 y 3, con timestamps de inicio y fin (`12:45 a 15:00` y `15:30 a 18:00`), objetos técnicos en infinitivo, evidencias verificables, blockers y planes de acción.

---

## 3. Prácticas de Semántica y Accesibilidad (WCAG)
Conforme a los requerimientos de la Guía GFPI-F-135 V04, el proyecto implementa:
- **Etiquetado Semántico Estricto:** `<header>`, `<nav>`, `<main>`, `<section>`, `<table>`, `<caption>`, `<thead>`, `<tbody>`, `<tr>`, `<th>`, `<td>`, `<footer>`.
- **Panel Superior de Navegación:** Menú principal `<nav aria-label="Menú principal de navegación">` en la parte superior de las tres vistas para saltar de forma inmediata entre páginas.
- **Identificación de Página Actual:** Atributo `aria-current="page"` para informar con precisión a los lectores de pantalla la ubicación del usuario.
- **Cuadrícula de Datos Accesible:** Todas las tablas cuentan con `<caption>` descriptivo y atributos de ámbito `scope="col"` y `scope="row"` para que las tecnologías de asistencia asocien cada dato a su encabezado.
- **Internacionalización:** Declaración explícita de idioma en `<html lang="es">`.

---

## 4. Enlaces de Entrega Oficial
- **Repositorio de Código Fuente:** [https://github.com/Marcosuarez02/Bitacora-HTML-ADSO](https://github.com/Marcosuarez02/Bitacora-HTML-ADSO)
- **Despliegue en Producción (GitHub Pages):** [https://marcosuarez02.github.io/Bitacora-HTML-ADSO/](https://marcosuarez02.github.io/Bitacora-HTML-ADSO/)
