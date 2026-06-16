# Caracterización de contribuyentes — Recaudo digital del Distrito de Medellín

Tablero ejecutivo que presenta el perfil del contribuyente del Distrito de Medellín y su disposición a migrar al canal virtual de recaudo, con la base estadística que respalda cada cifra. Pensado para lectura rápida del Secretario de Hacienda y las Subsecretarías de Tesorería, Ingresos y Presupuesto.

## Contenido

- **`index.html`** — Tablero completo. Es un archivo autocontenido: incluye los datos, los estilos, los gráficos (SVG/HTML nativos, sin librerías externas) y el logo institucional embebido. No requiere conexión a internet ni archivos adicionales para funcionar.
- **`.nojekyll`** — Indica a GitHub Pages que sirva el sitio tal cual, sin procesarlo con Jekyll.
- **`datos/caracterizacion.json`** — Las cifras que alimentan el tablero, por si se quieren auditar o actualizar.
- **`LICENSE.txt`** — Términos de uso.

## Qué muestra

1. **Validez estadística** — Población de 448.978 contribuyentes, muestra de 2.078 respuestas, margen de error real de ±2,1 % al 95 % de confianza, y los tamaños mínimos requeridos por escenario.
2. **El retrato del contribuyente** — Tipo (natural/jurídica), género, edad, estrato, dispositivos de pago, autonomía digital, uso previo del portal y retención en el canal virtual.
3. **Tres lecturas para la decisión** — Implicaciones de política de recaudo.

## Cómo desplegar en GitHub Pages

1. Crea un repositorio nuevo en GitHub (por ejemplo, `caracterizacion-recaudo`).
2. Sube **todos** los archivos de esta carpeta a la raíz del repositorio (incluido `index.html` y `.nojekyll`).
3. En el repositorio, ve a **Settings → Pages**.
4. En **Source**, elige la rama `main` (o `master`) y la carpeta `/ (root)`.
5. Guarda. En uno o dos minutos el sitio quedará publicado en:
   `https://<tu-usuario>.github.io/<nombre-del-repositorio>/`

> Si prefieres servir desde una subcarpeta, coloca los archivos en `/docs` y elige esa carpeta como *Source* en el paso 4.

## Cómo actualizar las cifras

Las cifras están escritas directamente en el objeto `D` dentro de `index.html` (busca `const D =`). Reemplaza los valores y vuelve a subir el archivo. El archivo `datos/caracterizacion.json` reproduce esas mismas cifras como referencia legible.

## Nota metodológica

La encuesta fue de respuesta voluntaria (tasa del 0,46 %) y la muestra se concentra en mayores de 56 años. Los porcentajes son robustos para el grupo encuestado; antes de extrapolar cifras puntuales a toda la población conviene ponderar por edad, estrato y tipo de contribuyente contra los registros del Distrito.

## Cumplimiento de identidad visual

El tablero usa la paleta y la tipografía del Manual de Identidad Visual de la Alcaldía de Medellín (V10). El logo se presenta respetando el área de protección. **Toda pieza con la marca está sujeta a validación de la Secretaría de Comunicaciones** antes de su publicación oficial.

---

**Desarrollado por:** Julián Alberto Uribe Gómez
**Supervisado por:** Jorge Iván Brand Ortiz
**Subsecretaría de Tesorería del Distrito de Medellín**

**Proyecto CTI:** Adopción tecnológica y analítica de datos orientados al fortalecimiento en la eficiencia del recaudo en la tesorería del distrito.
