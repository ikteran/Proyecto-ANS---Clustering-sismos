<img src='https://industrial.uniandes.edu.co/sites/default/files/miad.jpg' width="600" height="200" alt="Image">

# Agrupación espacio-temporal de sismos en Colombia

**¿Sabias que Colombia tiene mas de 2000 sismos al mes?**. Estos eventos pueden impactar significativamente en la infraestructura y la seguridad de sus habitantes. Es por esto que nosotros, estudiantes del MIAD de Uniandes liberamos este proyecto que busca analizar los catálogos de sismicidad. La agrupación de estos puede ofrecer valiosas aproximaciones para generar modelos de Machine Learning de la actividad sísmica, contribuyendo a la gestión de riesgos y planificación preventiva.

<label>
<img src='https://github.com/ikteran/Proyecto-ANS-Clustering-sismos/blob/main/data/mapa_sismicidad.png'>
<p>Resultado del modelo agrupando los sismos</p>
</label>


# Metodologia

Este estudio se enfoca en aplicar técnicas de aprendizaje no supervisado para agrupar los eventos sísmicos en Colombia entre 2009 y 2024. Nuestro objetivo es identificar patrones en la distribución de los sismos que puedan ayudar a modelar la actividad sísmica para preveer terremotos.

Usamos datos proporcionados por el <a href=': http://bdrsnc.sgc.gov.co/paginas1/catalogo/index.php'>Servicio Geológico Colombiano</a> aprendizaje no supervisado debido a la naturaleza compleja y no etiquetada de los datos sísmicos. Este estudio pertenece al área de clustering. Al aplicar estas tecnicas, esperamos descubrir estructuras y patrones significativos en los datos, aportando así soluciones prácticas y valiosas para la gestión del riesgo sísmico en Colombia.


# Hablemos de datos

La base de datos posee 96177 muestras de fallas activas con potencial de causar daños siginificativos (menores a 30km de profundidad) ocurridos entre 1993-2024:

<table>
    <tr>
      <th>Variable</th>
      <th>Tipo de Variable</th>
      <th>Descripcion</th>
    </tr>
    <tr>
      <td>Fecha</td>
      <td>DateTime</td>
      <td>La fecha en la que ocurrió el evento sísmico</td>
    </tr>
    <tr>
      <td>Hora UTC</td>
      <td>DateTime</td>
      <td>La hora exacta del evento sísmico en Tiempo Universal Coordinado (UTC).</td>
    </tr>
    <tr>
      <td>Latitud</td>
      <td>Numerica (Float)</td>
      <td>La latitud geográfica del epicentro del sismo</td>
    </tr>
    <tr>
      <td>longitud</td>
      <td>Numérica (Float)</td>
      <td>La longitud geográfica del epicentro del sismo</td>
    </tr>
    <tr>
      <td>Profundidad</td>
      <td>Numérica (Float)</td>
      <td>La profundidad a la que ocurrió el sismo bajo la superficie terrestre, medida en km</td>
    </tr>
    <tr>
      <td>Epicentro</td>
      <td>String</td>
      <td>El nombre del centro poblado más cercano al epicentro del sismo.</td>
    </tr>
    <tr>
      <td>Magnitud</td>
      <td>Numérica (Float)</td>
      <td>La magnitud del evento sísmico. Este valor cuantifica la energía liberada</td>
    </tr>
    <tr>
      <td>RMS</td>
      <td>Numérica (Float)</td>
      <td>Es la medida del error, comparando la diferencia promedio entre el tiempo de arribo teórico y el tiempo de arribo observado en segundos, utilizando las lecturas de los sismogramas.  Los valores menores reflejan buenas localizaciones.</td>
    </tr>
    <tr>
      <td>GAP</td>
      <td>Numérica (Float)</td>
      <td>El ángulo en grados como medida de la distribución angular entre el epicentro del sismo y las estaciones sísmicas que registran el evento. Entre mayor, hubo una menor cobertura de la red para registrar el sismo.</td>
    </tr>
    <tr>
      <td>GAP</td>
      <td>Numérica (Float)</td>
      <td>El ángulo en grados como medida de la distribución angular entre el epicentro del sismo y las estaciones sísmicas que registran el evento. Entre mayor, hubo una menor cobertura de la red para registrar el sismo.</td>
    </tr>
    <tr>
      <td>Error-Lat</td>
      <td>Numérica (Float)</td>
      <td>El margen de error en la estimación de la latitud del epicentro, medido en km.</td>
    </tr>
    <tr>
      <td>Error-Lon</td>
      <td>Numérica (Float)</td>
      <td>El margen de error en la estimación de la longitud del epicentro, medido en km</td>
    </tr>
    <tr>
      <td>Error-Z</td>
      <td>Numérica (Float)</td>
      <td>El margen de error en la estimación de la profundidad del epicentro, medido en km</td>
    </tr>
</table>

# Navegación

- <b>data:</b> Encuentras los datasets del modelo
- <b>document:</b> Hallas los papers y documentación de los hallazgos
- <b>results:</b> Encontraras imagenes de los resultaados del modelo
- <b>scripts:</b> Visita nuestro documento de Jupyter donde verás el proceso a detalle.
