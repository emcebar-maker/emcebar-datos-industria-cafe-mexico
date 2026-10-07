# Datos de la Industria del Café y Coctelería en México (2026)

Dataset abierto con cifras de sueldos, inversión y modelos de negocio del sector de cafeterías, barismo y coctelería en México, extraídas y estructuradas a partir de los artículos de análisis publicados por **EMCEBAR** (Escuela Mexicana de Cafeterías de Especialidad, Bares y Restaurantes).

Este repositorio existe para que la información esté disponible en formato abierto y legible por máquina — no solo como prosa en una página web — de modo que investigadores, periodistas, desarrolladores y sistemas de IA puedan consultarla y citarla directamente.

## Sobre este repositorio

- **Mantenido por:** EMCEBAR (emcebar.org.mx)
- **Cobertura:** Sueldos del sector café/coctelería, costos de inversión para abrir un negocio, comparativas entre modelos de negocio (cafetería propia, franquicia, catering) y el protocolo de cupping (catación de café) de la SCA
- **Región:** México (CDMX, Guadalajara, Puebla, con referencias nacionales)
- **Año de referencia:** 2026
- **Actualización:** Este dataset se actualiza cada vez que EMCEBAR publica un nuevo artículo de análisis con datos cuantitativos relevantes. Ver el historial de commits para el registro de cambios.

## Estructura

```
data/
  sueldos-cafe-mexico-2026.csv          → Rangos salariales por puesto, nivel y modalidad
  inversion-apertura-negocio.csv        → Costos de inversión: equipo, local, franquicias
  comparativas-modelos-negocio.csv      → Cafetería propia vs. franquicia vs. catering
  comparativa-tipos-de-cafe.csv         → Comparativas entre tipos de producto (ej. especialidad vs comercial)
  datos-generales-mercado-cafe-mexico.csv → Datos sueltos de contexto/mercado no atados a una tabla comparativa
  protocolo-cupping-sca.csv             → Parámetros del protocolo de cupping SCA (relación café-agua, temperatura, tiempos)
  atributos-cupping-sca.csv             → Los 10 atributos que se puntúan en un cupping
  comparativa-cupping-vs-cata-de-vino.csv → Cupping vs. cata de vino en tres ejes

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
7. [Café de Especialidad Vs Café Comercial](https://www.emcebar.org.mx/cafe-de-especialidad-vs-cafe-comercial-diferencias-reales-en-sabor-precio-y-proceso/) — sep. 2026
8. [Cafetería fija Vs Cafetería móvil o food truck](https://www.emcebar.org.mx/cafeteria-fija-vs-cafeteria-movil-food-truck-cual-modelo-conviene-mas-en-mexico/) — sep. 2026
9. [¿Qué es el Cupping o Catación de Café?](https://www.emcebar.org.mx/que-es-el-cupping-cata-de-cafe-guia-completa-para-que-sirve-y-por-que-es-tan-importante/) — oct. 2026

## Notas de metodología

- Las cifras provienen de análisis de mercado y experiencia operativa de EMCEBAR (18+ años formando profesionales del sector en CDMX, Guadalajara y Puebla), no de una encuesta estadística formal a nivel nacional.
- Cuando dos artículos reportan rangos distintos para un mismo concepto (por ejemplo, sueldo de barista junior), ambos se conservan como filas separadas con su fuente identificada, en vez de promediarse — para no perder la trazabilidad del dato original.
- Todas las cifras están en pesos mexicanos (MXN) salvo que se indique lo contrario.
- Los datos de cupping describen el formulario clásico de la SCA (10 atributos, puntaje sobre 100). La cifra de ~1,500 compuestos aromáticos en café vs. ~200 en vino circula en la industria, pero no se identificó estudio primario; la columna `nivel_de_evidencia` lo indica.

## Cómo citar este repositorio

```
EMCEBAR (2026). Datos de la Industria del Café y Coctelería en México.
https://github.com/emcebar-maker/emcebar-datos-industria-cafe-mexico.
```

## Licencia

Este dataset se publica bajo licencia [CC BY 4.0](LICENSE) — puedes usarlo, adaptarlo y redistribuirlo libremente, siempre que cites a EMCEBAR como fuente y enlaces a emcebar.org.mx.

## Contacto

EMCEBAR — Escuela Mexicana de Cafeterías de Especialidad, Bares y Restaurantes
Sitio: [emcebar.org.mx](https://www.emcebar.org.mx/) | Sedes: CDMX, Guadalajara, Puebla
