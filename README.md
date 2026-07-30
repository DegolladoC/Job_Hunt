# JobQuest — Dashboard público

JobQuest es un dashboard de estadísticas sobre la búsqueda de trabajo de **Dego**.

Este repositorio contiene únicamente la visualización pública y archivos de datos agregados. El desarrollo completo, las automatizaciones y la información individual permanecen en un entorno privado.

> Estado: el dashboard público está en proceso de adaptación. Los datos visibles durante esta etapa pueden ser demostrativos y no deben interpretarse como actividad actual.

## Qué mostrará el dashboard

El dashboard permitirá consultar periodos semanales, mensuales e históricos.

### Resumen general

- Total de postulaciones.
- Total de respuestas.
- Tasa de respuesta.
- Cantidad de entrevistas.
- Cantidad de ofertas.
- Variación frente al periodo anterior.

### Embudo de búsqueda

Conteos agregados por etapa:

- Postulación enviada.
- Confirmación recibida.
- Contacto humano.
- Evaluación.
- Entrevista.
- Oferta.
- Rechazo o proceso cerrado.

### Actividad y tendencias

- Postulaciones por día de la semana.
- Tendencia semanal y mensual.
- Respuestas por periodo.
- Tiempo de respuesta expresado como rango o mediana.

### Eficiencia

Se mostrarán postulaciones, respuestas, entrevistas y tasas agregadas por:

- Plataforma de empleo.
- Alias de CV.
- Categoría general de puesto.
- Rango salarial.
- Modalidad: remoto, híbrido o presencial.

Los CV usarán alias descriptivos como `CV-Automatización` o `CV-Datos`; nunca se publicarán nombres de archivos ni documentos personales.

### Empresas repetidas

No se mostrarán nombres de empresas. Esta sección se limitará a:

- Cantidad de empresas con postulaciones repetidas.
- Distribución de una, dos, tres o más postulaciones.
- Comparación agregada entre primeras postulaciones y postulaciones repetidas.

### Calidad de la información

- Registros analizados.
- Porcentaje de registros completos.
- Fecha de actualización.
- Advertencias cuando la muestra sea insuficiente.

## Protección de privacidad

En este sitio, el usuario será identificado únicamente como **Dego**.

La publicación bloqueará:

- Nombres completos y apellidos.
- Nombres de empresas asociadas con postulaciones.
- Nombres de reclutadores, contactos o clientes.
- Teléfonos, WhatsApp, correos y direcciones.
- Matrículas, folios e identificadores.
- URL de vacantes.
- Fechas exactas vinculadas con una postulación.
- Puestos exactos asociados con una empresa.
- Salarios exactos.
- CV, cartas, notas y mensajes.
- Registros individuales de postulaciones o entrevistas.
- Tokens, contraseñas y credenciales.

Los nombres de pila de terceros solo podrán utilizarse cuando sean necesarios, no identifiquen una postulación y exista autorización. Por defecto no se publicarán nombres de terceros.

Los números estadísticos —conteos, porcentajes, tendencias y rangos— sí podrán mostrarse. Los números personales o identificadores permanecerán bloqueados.

## Reglas estadísticas

- Solo se publicarán datos agregados.
- Los grupos con menos de cinco registros mostrarán `Muestra insuficiente`.
- Se utilizarán categorías de puesto, no títulos exactos.
- Los salarios se expresarán mediante rangos amplios.
- Las fechas se mostrarán como periodos generales.
- Cualquier campo no autorizado detendrá la publicación automática.

## Separación de datos

```text
Datos privados
      |
      v
Generación de estadísticas
      |
      v
Validación y sanitización
      |
      v
Job_Hunt / GitHub Pages
```

Este repositorio no es la fuente de verdad ni almacena los datos crudos. Recibe únicamente los artefactos públicos que hayan superado la validación de privacidad.
