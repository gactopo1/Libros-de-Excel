# Herramientas geodesicas en Excel

Este repositorio reúne libros de Excel con Macros (VBA) para proyeccion y transformación de coordenadas.

---

## 1. TransCoordArg - Transformación de Coordenadas.
Herramienta diseñada para la conversión precisa de coordenadas dentro del territorio argentino. Posgar04, Posgar07, Campo Inschauspe 69, PASMA, TDF95, Tapi Aike, Chos Malal 1914, Pampa del Castillo, MMN , MMS, Yavi, Carranza, Castelli, 25 de Mayo, Ubajay, Sistemas provinciales

**Formatos:** Transformación entre coordenadas geográficas y planas (Gauss-Krüger).
**Uso Local:** Parámetros ajustados específicamente para la República Argentina.
**Macros:** Utiliza código VBA para procesar cálculos matemáticos complejos.

## 2. Proyecciones
Recopilación de ecuaciones para la solución de diversas proyecciones cartográficas, desarrolladas en Excel y programadas íntegramente en VBA.

<details>
<summary><b>Ver lista completa de proyecciones soportadas (Click para desplegar)</b></summary>

### Azimuthal & Perspective
* Airy
* Aitoff
* Azimuthal Equidistant (Equatorial, Oblique, Polar)
* Gnomonic (Equatorial, Oblique, Polar)
* Orthographic & Perspective (Vertical, Tilted, Camera Parameters)
* Stereographic (Polar, Equatorial, Oblique - Variant A, B, C)
* Universal Polar Stereographic (UPS)

### Cylindrical
* Cassini & Cassini-Soldner
* Central Cylindrical
* Cylindrical Equal Area (Behrmann, Gall, Lambert, Smyth)
* Equidistant Cylindrical (Plate Carrée)
* Mercator (Spherical, 2SP, Web Mercator, Pseudo-Mercator)
* Transverse Mercator (UTM, Gauss-Krüger, Gauss-Boaga, South Orientated)
* Miller Cylindrical I & II

### Conic & Polyconic
* Albers Equal Area (1SP, 2SP)
* Equidistant Conic
* Lambert Conformal Conic (1SP, 2SP, Belgium 72)
* Polyconic (American, Rectangular, Ginzburg)
* Krovak (Modified, North Orientated)

### Pseudocylindrical & Others
* Eckert I - VI
* Mollweide & Goode Homolosine
* Robinson & Natural Earth I/II
* Sinusoidal (Sanson-Flamsteed)
* Wagner I - VII
* Winkel Tripel
* Bonne & Werner

*(Y más de 100 variantes adicionales incluidas en el libro de Excel)*
</details>

---

## 3. Transformación de Datum (Bursa-Wolf 7P & Helmert 10P)
Herramienta avanzada para la estimación y aplicación de parámetros de transformación...
---
## 3. Transformación de Datum (Bursa-Wolf & Helmert 3D)
Herramienta avanzada para la estimación y aplicación de parámetros de transformación entre marcos de referencia, utilizando un motor de álgebra lineal desarrollado íntegramente en VBA.
## Modelos Implementados:
**. Bursa-Wolf (7 Parámetros):** Modelo geocéntrico estándar que utiliza 3 traslaciones, 3 rotaciones y 1 factor de escala. Las rotaciones se ejecutan respecto al origen del sistema (Centro de Masas).
**. Helmert / Molodensky-Badekas (10 Parámetros):** Modelo de alta precisión para áreas locales. Incluye los 7 parámetros clásicos más las 3 coordenadas del baricentro local como punto de rotación. Esto elimina la correlación entre traslación y rotación, otorgando mayor estabilidad a los parámetros en proyectos de ingeniería.
## Características Técnicas:
**. Motor Autónomo:** Incluye funciones propias para inversión de matrices por Gauss-Jordan (InvMatrizGJ), productos matriciales y transposición. No requiere librerías externas.
**. Ajuste por Mínimos Cuadrados:** Estimación de parámetros a partir de puntos de control.Cálculo de Residuales: Análisis automático de errores residuales ($V = AX - Y$) para auditar la precisión de cada punto transformado.
**. Convención:** Implementa el estándar internacional Position Vector Transformation.

## ⚠️ Requisitos y Seguridad
Libros habilitados para macros (`.xlsm`).

1. **Habilitar Contenido:** Al abrir los archivos, debe aceptar el uso de Macros para que las funciones de cálculo se activen.
2. **Desbloqueo de Windows:** Si el archivo no ejecuta las funciones, haga clic derecho sobre el archivo en su carpeta, vaya a **Propiedades** y marque la casilla **"Desbloquear"**.
3. **Entorno de Programación:** Para ver el código fuente, presione ALT + F11. Los algoritmos matemáticos se encuentran en el Módulo 1.
## 🚀 Cómo utilizar
1. Descargue el repositorio o el archivo específico que necesite.
2. Para Proyecciones: Ingrese los datos en las celdas de entrada (marcadas en celeste).
3. Para Transformación de Datum: Ingrese sus puntos de control en la Hoja 1 para calcular los parámetros; luego aplíquelos en la Hoja 2 utilizando el método matricial o lineal.
4. 
---

## 📥 Descargas Directas

* 📄 **[Descargar TransCoordArg.xlsm](https://github.com/gactopo1/Libros-de-Excel/raw/main/TransCoordArg.xlsm)**
* 📄 **[Descargar Proyecciones.xlsm](https://github.com/gactopo1/Libros-de-Excel/raw/main/Proyecciones.xlsm)**
* 📄 **[Descargar Transformación de Datum (Bursa-Wolf - 7 Parámetros)](https://github.com/gactopo1/Libros-de-Excel/raw/main/Transformaci%C3%B3n%20de%20Datum%20y%20calculo%20de%20parametros%20-%20Bursa-Wolf.xlsm)**
* 📄 **[Descargar Transformación de Datum (Helmert/Molodensky-Badekas - 10 Parámetros)](https://github.com/gactopo1/Libros-de-Excel/raw/main/Transformaci%C3%B3n%20de%20Datum%20-%20Helmert%203D%20y%20calculo%20de%20parametros%20-%20Molodensky-Badecas.xlsm)**
* 
**Palabras clave:** Excel, Argentina, EPSG, Coordenadas, Geodesia, Agrimensura, Gauss-Krüger, Transformación de Datums, Bursa-Wolf, Helmert, Molodensky-Badecas, GIS, VBA, Proyecciones Cartográficas.
