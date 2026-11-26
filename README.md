# Portafolio de series de tiempo

**Autor:** Luca Lagos Paciello · Examen del viernes 27 de noviembre

Cuatro proyectos de series de tiempo, uno por herramienta. Cada carpeta tiene su código o archivo, sus datos y los resultados.

| # | Carpeta | Herramienta | Serie | Frecuencia |
|---|---------|-------------|-------|------------|
| 1 | `01_Python_TPM` | Python (Jupyter/Colab) | Tasa de Política Monetaria (TPM) | Diaria, 2020 – ago 2026 |
| 2 | `02_R_IMACEC_no_minero` | R (Jupyter/Colab) | IMACEC no minero, base 2018=100 | Mensual, 164 observaciones |
| 3 | `03_PowerBI_Rumbo_Norte` | Power BI Desktop | Ventas de Rumbo Norte | Transacciones 2024–2025 |
| 4 | `04_Tableau_Rumbo_Norte` | Tableau | Ventas de Rumbo Norte | Transacciones 2024–2025 |

## 1. Python · TPM
- **Qué hace:** limpia el archivo (fecha y TPM venían en una sola columna), ordena la serie y grafica su evolución.
- **Cómo abrirlo:** abrir `codigo/Reporte1_TPM.ipynb` en Google Colab, subir `TPM.xlsx` (ver `datos/`) y ejecutar todo.
- **Hallazgo:** mínimo de 0,5% (2020–2021), máximo de 11,25% a fines de 2022 y 4,5% a mediados de 2026.

## 2. R · IMACEC no minero
- **Qué hace:** serie con promedio móvil de 12 meses, mapa de calor año × mes y variación interanual.
- **Cómo abrirlo:** abrir `codigo/IMACEC_no_minero.ipynb` en Colab con kernel de R, subir el Excel del IMACEC (ver `datos/`) y ejecutar. Los PNG generados están en la carpeta.
- **Hallazgo:** −17,5% interanual en mayo 2020, +23,4% en junio 2021 y bajo dinamismo en 2026.

## 3. Power BI · Rumbo Norte
- **Qué hace:** modelo estrella (Productos, Sucursales, Ventas) con medidas de ventas, ticket promedio y margen.
- **Cómo abrirlo:** abrir `codigo/Caso_07_Lagos.pbix` en Power BI Desktop. Si pide actualizar la fuente, apuntar a `datos/Caso_07_Rumbo_Norte_Sabana_de_datos.xlsx`.
- **Informe:** `Informe_Ejecutivo_PowerBI.docx`.
- **Hallazgo:** ventas +37,4% en 2025; Providencia cae −96,4% en agosto 2025.

## 4. Tableau · Rumbo Norte
- **Qué hace:** dashboard con indicadores, evolución mensual, comparación por categoría, sucursal y producto.
- **Cómo abrirlo:** abrir `codigo/Caso_07_Rumbo_Norte_Dashboard.twbx` en Tableau Desktop o Tableau Public. Los datos van incluidos en el libro.
- **Informe:** `Informe_Ejecutivo_Tableau.docx`.
- **Hallazgo:** Internacionales aporta 47,7% de las ventas y 65,7% de la utilidad; Chiloé 3 días tiene margen de 4,9%.

## Estructura
```
01_Python_TPM/  02_R_IMACEC_no_minero/  03_PowerBI_Rumbo_Norte/  04_Tableau_Rumbo_Norte/
└── codigo/ (notebook, .pbix o .twbx)   └── datos/ (Excel o link a la fuente)
```
