# framings

**framings** es un proyecto de análisis hemerográfico y mediático orientado a la **observación de encuadres** (*media framing*) desde una perspectiva de **segundo orden**. No busca resumir noticias ni producir síntesis informativas tradicionales, sino **hacer visible cómo los medios observan, jerarquizan y narran los acontecimientos**.

El proyecto parte de una premisa simple pero exigente: *un mismo evento no existe de forma unívoca en el espacio público; existe como una constelación de observaciones*. **framings** archiva, organiza y compara esas observaciones.

---

## ¿Qué hace este repositorio?

- Reorganiza seguimientos de prensa (portadas y artículos) como **datasets estructurados**.
- Separa claramente:
  - el **hecho**,
  - su **tratamiento mediático**,
  - y la **lectura analítica**.
- Permite comparar **encuadres**, **tonos**, **jerarquías** y **supuestos implícitos** entre medios.
- Funciona como **base de datos legible por humanos y por modelos de lenguaje (LLMs)**.

Este repositorio **no es un producto final**, sino un **dispositivo analítico reutilizable**.

---

## Enfoque conceptual

**framings** se apoya en:

- *Frame analysis* (Goffman, Entman)
- Observación de segundo orden (Luhmann)
- Estudios críticos de medios
- Análisis discursivo y visual de la prensa

El interés central no es *qué ocurrió*, sino:

> **cómo fue observado, qué fue enfatizado, qué fue desplazado y bajo qué supuestos se construyó sentido**.

---

## Estructura del repositorio

```
framings/
├── datasets/
│   └── trump-venezuela_2025-12-17/
│       ├── dataset.yaml
│       ├── content/
│       │   ├── dia.md
│       │   ├── *_portada.md
│       │   ├── articulo_*.md
│       │   └── comparativo.md
│       └── images/
│
├── templates/          # esquemas reutilizables (YAML + MD)
├── scripts/            # (opcional) utilidades futuras
└── README.md
```

### Componentes clave

- **`dataset.yaml`**  
  Archivo estructural. Define relaciones, jerarquías, metadatos y rutas. No contiene texto largo.

- **`content/*.md`**  
  Archivos analíticos en Markdown: observación de portadas, artículos y comparativos.

- **`images/`**  
  Material visual (portadas, recortes). Referenciado desde YAML, no incrustado.

---

## Principios de trabajo

1. **Separación estricta entre estructura y contenido**  
   El YAML ordena; el Markdown observa.

2. **Un evento, múltiples encuadres**  
   Cada medio se registra como una observación distinta, no como una variación menor.

3. **Comparabilidad antes que exhaustividad**  
   Se prioriza la claridad analítica sobre el volumen de información.

4. **Legibilidad humana + procesabilidad algorítmica**  
   El repositorio está pensado tanto para lectura crítica como para generación posterior de visualizaciones o sitios web.

---

## ¿Para qué sirve?

- Crear **archivos comparativos de cobertura mediática**.
- Diseñar **sitios web, timelines o mapas de encuadres** a partir de los datasets.
- Entrenar o evaluar LLMs en análisis de framing sin ambigüedad estructural.
- Apoyar investigación académica, docencia o análisis político-mediático.

---

## Estado del proyecto

- 🟢 Fase inicial
- Primer dataset piloto completamente estructurado
- Esquema replicable por día, tema o evento

---

## Licencia y uso

El contenido analítico es de uso académico y crítico.  
Las imágenes de portadas pertenecen a sus respectivos medios y se incluyen solo con fines de análisis.

---

## Nota final

**framings** no pretende decirle al lector *qué pensar*, sino mostrarle **cómo ya se le está invitando a pensar**.

Ese es su gesto político y epistemológico.

