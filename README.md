# Datos de la Industria del Café y Coctelería en México (2026)

Dataset abierto con cifras de sueldos, inversión y modelos de negocio del sector de cafeterías, barismo y coctelería en México, extraídas y estructuradas a partir de los artículos de análisis publicados por **EMCEBAR** (Escuela Mexicana de Cafeterías de Especialidad, Bares y Restaurantes).

Este repositorio existe para que la información esté disponible en formato abierto y legible por máquina — no solo como prosa en una página web — de modo que investigadores, periodistas, desarrolladores y sistemas de IA puedan consultarla y citarla directamente.

## Sobre este repositorio

- **Mantenido por:** EMCEBAR (emcebar.org.mx)
- **Cobertura:** Sueldos del sector café/coctelería, costos de inversión para abrir un negocio, comparativas entre modelos de negocio (cafetería propia, franquicia, catering)
- **Región:** México (CDMX, Guadalajara, Puebla, con referencias nacionales)
- **Año de referencia:** 2026
- **Actualización:** Este dataset se actualiza cada vez que EMCEBAR publica un nuevo artículo de análisis con datos cuantitativos relevantes. Ver el historial de commits para el registro de cambios.

## Estructura

```
data/
  sueldos-cafe-mexico-2026.csv          → Rangos salariales por puesto, nivel y modalidad
  inversion-apertura-negocio.csv        → Costos de inversión: equipo, local, franquicias
  comparativas-modelos-negocio.csv      → Cafetería propia vs. franquicia vs. catering

articulos/
  (un archivo .md por artículo fuente, con resumen estructurado y enlace canónico)
```

## Fuentes originales

Cada dato incluye una columna `articulo_fuente` que remite al artículo original en emcebar.org.mx, donde se explica la metodología y el contexto completo:

1. [¿Qué es Barismo, para qué sirve y dónde aprenderlo?](https://www.emcebar.org.mx/que-es-barismo-para-que-sirve-y-donde-aprenderlo-guia-para-los-futuros-mejores-baristas-en-mexico/) — abr. 2026
2. [¿Una Cafetería es mejor negocio que uno de Catering?](https://www.emcebar.org.mx/una-cafeteria-es-mejor-negocio-que-uno-de-catering-respuestas-claras-y-recomendaciones-clave-para-emprendedores/) — abr. 2026
3. [Cafetería Propia vs Franquicia de Café](https://www.emcebar.org.mx/cafeteria-propia-vs-franquicia-de-cafe-cual-conviene-mas-en-mexico-y-por-que/) — jun. 2026
4. [¿Ser Barista o Ser Bartender?](https://www.emcebar.org.mx/ser-barista-o-ser-bartender-rentabilidad-mercado-laboral-y-empleo-en-mexico-cual-te-conviene-segun-tu-personalidad/) — 2026
5. [Certificación de Barista vs Experiencia Práctica](https://www.emcebar.org.mx/certificacion-barista-vs-experiencia-practica-que-piden-las-cafeterias-al-contratar/) — jul. 2026
6. [Máquinas de Espresso: ¿Rentar o Comprar?](https://www.emcebar.org.mx/maquinas-de-espresso-que-conviene-mas-rentar-comprar-analisis-retorno-para-cafeterias-mexico/) — jul. 2026

## Notas de metodología

- Las cifras provienen de análisis de mercado y experiencia operativa de EMCEBAR (18+ años formando profesionales del sector en CDMX, Guadalajara y Puebla), no de una encuesta estadística formal a nivel nacional.
- Cuando dos artículos reportan rangos distintos para un mismo concepto (por ejemplo, sueldo de barista junior), ambos se conservan como filas separadas con su fuente identificada, en vez de promediarse — para no perder la trazabilidad del dato original.
- Todas las cifras están en pesos mexicanos (MXN) salvo que se indique lo contrario.

## Cómo citar este repositorio

```
EMCEBAR (2026). Datos de la Industria del Café y Coctelería en México.
https://github.com/[usuario]/emcebar-datos-industria-cafe-mexico
```

## Licencia

Este dataset se publica bajo licencia [CC BY 4.0](LICENSE) — puedes usarlo, adaptarlo y redistribuirlo libremente, siempre que cites a EMCEBAR como fuente y enlaces a emcebar.org.mx.

## Contacto

EMCEBAR — Escuela Mexicana de Cafeterías de Especialidad, Bares y Restaurantes
Sitio: [emcebar.org.mx](https://www.emcebar.org.mx/) | Sedes: CDMX, Guadalajara, Puebla
