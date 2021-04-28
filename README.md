# Crossfilter Example

Copiado online y le introduje una nueva base de datos

## Paso 1

Ingrese al directorio "ENAHO-master"

## Paso 2

Ejecute

	bokeh serve --show --port 8899  crossfilter

	bokeh serve --show crossfilter
    
# Sobre la metodología de Statistical Learning (Aprendizaje estadístico) que actúa sobre la base de datos del INEC: Bayesian inference on a hierarchical mixed model
    

## Objetivo
1. **Mixed** Extraer *proxies* (indicadores, índices) de variables de diseño de la *encuesta compleja* (como en los ensayos clínicos de la vacuna COVID): REGION, ZONA y DENSIDAD_POBLACIONAL para calibrar las observaciones (personas encuestadas). Este paso es necesario pues una encuesta **no** es un censo de toda la población, si no de subpoblaciones. 

Ejemplo: encuestar 10 ramonenses es tan representativo como encuestar 1 esparzano pues la proporción de SanRamón:Esparza = 10:1.

2. **Hierarchical** Reconocer la institucionalidad socioeconómica compartida por las y los individuos (*pooling observations*) a través de distintos lentes: REGION, ZONA y DENSIDAD_POBLACIONAL.

Ejemplo: ramonenses y alajuelenses pertenecen a la misma REGION pero distinta ZONA. Así, la institucionalidad socioeconómica que mide la ENAHO les afecta distinto. (La curvatura de regiones isotrópicas es distinta: la institucionalidad actúa de modo distinto en distintas localidades.)

3. **Bayesian** Incertidumbre asociada en la evidencia. Responde a las preguntas: ¿Cuánto podemos confiar en los datos que *midió* el INEC mediante la encuesta? Principio de incertidumbre de Heisenberg: **momentum** del ingreso determina su evolución, mientras que la **posición** del ingreso es cuánto mide en un momento determinado. 

# Siguientes mejoras del software:

## Mejoras en deployment:

1. Aumentar cantidad de variables que se pueden visualizar en 4-dimensiones.

Necesitamos: capacidad de procesamiento: AWS, Googl	e

Mi computadora está desgastada.  (No sirve)

2. Subirlo a la web (online)

3. Escalabilidad (democratizar la lectura sobre la situación de los hogares)

4. Público meta: ¿PAC, UCR, Laura o Asamblea?


## Mejoras en metodología

1. Tomar en consideración incertidumbre en la medición del INEC (coeficiente de variación).

2. Incluir regresiones multivariable de todas las demás 500 variables medidas.
