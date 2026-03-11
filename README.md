<div align="center">
  <img width="100%" height="220" src="https://capsule-render.vercel.app/api?type=waving&color=0:0a192f,50:112240,100:233554&height=220&section=header&text=Marco%20Oviedo&fontSize=80&animation=fadeIn&fontAlignY=35&desc=Data%20Engineer%20%7C%20Financial%20Analytics%20%7C%20BI%20Automation&descAlignY=55&descAlign=62&fontColor=64ffda" alt="header"/>
</div>

<p align="center">
  <a href="https://git.io/typing-svg">
    <img src="https://readme-typing-svg.demolab.com?font=JetBrains+Mono&weight=500&size=22&duration=3500&pause=1000&color=64FFDA&center=true&vCenter=true&multiline=false&repeat=infinity&width=700&height=45&lines=Building+financial+data+pipelines+at+scale;Automating+what+shouldn't+be+manual;From+Oracle+GL+to+executive+dashboards" alt="Typing SVG" />
  </a>
</p>

<div align="center">
  
  [![LinkedIn](https://img.shields.io/badge/LinkedIn-Marco%20Oviedo-0077B5?style=flat-square&logo=linkedin&logoColor=white)](https://linkedin.com/in/marco-oviedo-992a321a9)
  ![Profile Views](https://komarev.com/ghpvc/?username=oviedomarco&color=64ffda&style=flat-square)
  
</div>

---

### Quién soy

Soy **Data Engineer** en **Farmacias del Ahorro**, donde construyo y mantengo los pipelines de datos financieros que alimentan los reportes ejecutivos de la organización — P&L, Balance General, Capital de Trabajo y analíticos de gasto por farmacia.

Mi trabajo diario vive en la intersección de **ingeniería de datos** y **finanzas corporativas**: extraer datos de Oracle GL, transformarlos en una arquitectura medallion (Bronze → Silver → Gold), y entregar reportes automatizados en Power BI, Excel y PowerPoint que antes tomaban días de trabajo manual.

Paralelamente, estudio **Actuaría** en la **Universidad Autónoma de Nuevo León (UANL)** y sigo una ruta autodidacta en matemáticas, finanzas cuantitativas y fundamentos de ingeniería de datos.

---

### 🔧 Stack real — lo que uso todos los días

<table>
<tr>
<td valign="top" width="33%">

**Datos & Pipelines**

![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white)
![Polars](https://img.shields.io/badge/Polars-CD792C?style=flat-square&logo=polars&logoColor=white)
![SQL](https://img.shields.io/badge/SQL-4479A1?style=flat-square&logo=oracle&logoColor=white)
![Parquet](https://img.shields.io/badge/Parquet-50ABF1?style=flat-square&logoColor=white)
![Selenium](https://img.shields.io/badge/Selenium-43B02A?style=flat-square&logo=selenium&logoColor=white)
![YAML](https://img.shields.io/badge/YAML-CB171E?style=flat-square&logo=yaml&logoColor=white)

</td>
<td valign="top" width="33%">

**BI & Reporting**

![Power BI](https://img.shields.io/badge/Power_BI-F2C811?style=flat-square&logo=power-bi&logoColor=black)
![DAX](https://img.shields.io/badge/DAX-F2C811?style=flat-square&logoColor=black)
![Excel](https://img.shields.io/badge/Excel_/_VBA-217346?style=flat-square&logo=microsoft-excel&logoColor=white)
![PowerPoint](https://img.shields.io/badge/PowerPoint_Auto-B7472A?style=flat-square&logo=microsoft-powerpoint&logoColor=white)

</td>
<td valign="top" width="33%">

**Infraestructura**

![Oracle](https://img.shields.io/badge/Oracle_GL-F80000?style=flat-square&logo=oracle&logoColor=white)
![Git](https://img.shields.io/badge/Git-F05032?style=flat-square&logo=git&logoColor=white)
![Obsidian](https://img.shields.io/badge/Obsidian-7C3AED?style=flat-square&logo=obsidian&logoColor=white)

</td>
</tr>
</table>

---

### 📐 Arquitectura de trabajo

```
                    ┌─────────────────────────────────────────────┐
                    │            ORACLE GL / DISCOVERER            │
                    └──────────────────┬──────────────────────────┘
                                       │  Selenium + Python
                                       ▼
                    ┌─────────────────────────────────────────────┐
                    │              🥉 BRONZE LAYER                │
                    │         Raw extracts → Parquet files        │
                    └──────────────────┬──────────────────────────┘
                                       │  Polars lazy API
                                       ▼
                    ┌─────────────────────────────────────────────┐
                    │              🥈 SILVER LAYER                │
                    │   Dimension tables + Config-driven transforms│
                    │   YAML closure schedule, store status logic  │
                    └──────────────────┬──────────────────────────┘
                                       │  Aggregation + business rules
                                       ▼
                    ┌─────────────────────────────────────────────┐
                    │              🥇 GOLD LAYER                  │
                    │  P&L  │  Balance  │  WC  │  Expense Reports │
                    └──────────┬──────────┬───────────┬───────────┘
                               │          │           │
                          Power BI    Excel/XLSX   PowerPoint
```

---

### 🏗️ Proyectos principales

| Proyecto | Descripción | Tech |
|----------|-------------|------|
| **`financial-planning`** | Arquitectura medallion completa para planeación financiera. Pipelines de presupuesto, dimensiones (sucursales, cuentas, centros de costo), clasificación dinámica de tiendas (Mismas vs Nuevas) con YAML config. | `Python` `Polars` `Parquet` `YAML` |
| **Expense Report Generator** | Generador automatizado de 6 archivos XLSX por categoría de gasto con tablas comparativas YTD (actual vs año anterior, actual vs presupuesto, TT vs TM). | `Python` `Polars` `openpyxl` |
| **Oracle GL Extractor** | Bot de Selenium que extrae reportes GL Auxiliar de Oracle Discoverer con mapeo completo de 20 campos de formulario. | `Python` `Selenium` |
| **WC Weekly Pipeline** | Pipeline de Capital de Trabajo con salidas automatizadas en PowerPoint, PDF y Excel. Arquitectura clean-slate. | `Python` `pptx` `Polars` |
| **Power BI Financial Suite** | Dashboard financiero con P&L, disconnected layout tables, parameter slicers, y tema Navy personalizado alineado a NIFs mexicanas. | `Power BI` `DAX` |

---

### 📚 En qué estoy invirtiendo

```python
learning_path = {
    "matemáticas":  ["Álgebra de Baldor", "Spivak → Cálculo", "Álgebra Lineal"],
    "finanzas":     ["Corporate Finance (currículo 24 meses)", "Microeconomía (Varian)"],
    "data_eng":     ["Fundamentals of Data Engineering (Reis & Housley)"],
    "universidad":  ["UANL — Actuaría"],
}
```

---

### 🎯 Hacia dónde voy

Mi objetivo a largo plazo es ser el puente entre **ingeniería de datos** y **finanzas corporativas** — un perfil que en México es raro y valioso. No soy un data scientist genérico; soy alguien que entiende un Estado de Resultados, sabe construir el pipeline que lo alimenta, y puede automatizar su entrega de punta a punta.

---

<div align="center">

### 📊 GitHub Stats

<img height="170" src="https://github-readme-stats.vercel.app/api?username=oviedomarco&show_icons=true&theme=react&bg_color=0a192f&title_color=64ffda&icon_color=64ffda&text_color=8892b0&border_color=112240&hide_border=false" />
<img height="170" src="https://github-readme-stats.vercel.app/api/top-langs/?username=oviedomarco&layout=compact&theme=react&bg_color=0a192f&title_color=64ffda&text_color=8892b0&border_color=112240&hide_border=false" />

</div>

---

<div align="center">
  
  <img width="100%" src="https://capsule-render.vercel.app/api?type=waving&color=0:0a192f,50:112240,100:233554&height=100&section=footer&fontColor=64ffda" alt="footer"/>

  <sub>Built with honesty, not with hype.</sub>
  
</div>
