<p align="center">
  <img src="https://industrial.uniandes.edu.co/sites/default/files/miad.jpg" width="300" height="100" alt="Image">
</p>

# Agrupación espacio-temporal de sismos en Colombia

**¿Sabías que Colombia tiene más de 2000 sismos al mes?** Estos eventos pueden impactar significativamente en la infraestructura y la seguridad de sus habitantes. Por ello, nosotros, estudiantes del MIAD de Uniandes, hemos desarrollado este proyecto para analizar los catálogos de sismicidad. La agrupación de estos eventos puede ofrecer valiosas perspectivas para generar modelos de Machine Learning sobre la actividad sísmica, contribuyendo así a la gestión de riesgos y a la planificación preventiva.

<p align="center"> <img src="https://github.com/ikteran/Proyecto-ANS-Clustering-sismos/blob/main/data/mapa_sismicidad.png" width="300" height="400" alt="Distribución espacial de los datos de sismicidad utilizados en el proyecto"> <br> <small>Distribución espacial de los datos de sismicidad utilizados en el proyecto</small> </p>


# Metodología

Este estudio se enfoca en aplicar técnicas de aprendizaje no supervisado para agrupar los eventos sísmicos en Colombia entre 2009 y 2024. Nuestro objetivo es identificar patrones en la distribución de los sismos que puedan ayudar a modelar la actividad sísmica.

Utilizamos datos proporcionados por el <a href="http://bdrsnc.sgc.gov.co/paginas1/catalogo/index.php">Servicio Geológico Colombiano</a>. Optamos por el aprendizaje no supervisado debido a la naturaleza compleja y no etiquetada de los datos sísmicos. Este estudio se enmarca en el área de clustering. Al aplicar estas técnicas, esperamos descubrir estructuras y patrones significativos en los datos, aportando así soluciones prácticas y valiosas para la gestión del riesgo sísmico en Colombia.


# Hablemos de datos

La base de datos contiene 96177 resgistros sísmicos superficiales (menor a 30km de profundidad), los cuales son interesantes ya que tienen un mayor potencial de causar daños siginificativos. A continuación se describen las variables:

<table>
    <tr>
      <th>Variable</th>
      <th>Tipo de Variable</th>
      <th>Descripción</th>
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

- <b>data:</b> Se encuentra la base de datos utilizada en formato csv
- <b>document:</b> Está la documentación de los hallazgos
- <b>results:</b> Se encuentran los archivos e imagenes obtenidas a partir de los resultados
- <b>scripts:</b> Visita nuestro documento de Jupyter donde verás el proceso a detalle.

# Referencias

A continuación, te compartimos algunos artículos científicos que exploramos para este proyecto:

<ol>
<li><strong>Gracia, M. D.</strong> (2017). <em>Seismotectonic characterization of the Colombian Pacific region: Identification of tectonic patterns through geostatistical analysis</em> (Undergraduate thesis). Universidad de los Andes, School of Sciences, Faculty of Geosciences.</li>

<li><strong>Mato, F., & Toulkeridis, T.</strong> (2017). An unsupervised K-means based clustering method for geophysical post-earthquake diagnosis. <em>2017 IEEE Symposium Series on Computational Intelligence (SSCI)</em>, 1–8. <a href="https://doi.org/10.1109/SSCI.2017.8285216" target="_blank">https://doi.org/10.1109/SSCI.2017.8285216</a></li>

<li><strong>Novianti, P., Setyorini, D., & Rafflesia, U.</strong> (2017). K-Means cluster analysis in earthquake epicenter clustering. <em>International Journal of Advances in Intelligent Informatics</em>, 3(2), 81. <a href="https://doi.org/10.26555/ijain.v3i2.100" target="_blank">https://doi.org/10.26555/ijain.v3i2.100</a></li>

<li><strong>Yuan, R.</strong> (2021). An improved K-means clustering algorithm for global earthquake catalogs and earthquake magnitude prediction. <em>Journal of Seismology</em>, 25(3), 1005–1020. <a href="https://doi.org/10.1007/s10950-021-09999-8" target="_blank">https://doi.org/10.1007/s10950-021-09999-8</a></li>
</ol>

