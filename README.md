# Seguimiento-1
## Pregunta 1: 
Describa los campos que se encontrará en este tipo de archivos. ¿Qué información está allí contenida? Proporcione ejemplos.

Los archivos GFF3 se basan en la descripción de características de genes  y viene de un tipo de archivo GFF (General Feature Format) que busca organizar esta información en columnas y separado por el espacio tab, sin embargo, GFF3 se considera una evolución de este mecanismo ya que permite entregar anotaciones más detalladas de lo que se describe al igual que incluye nuevas herramientas como más niveles para agrupamiento jerárquico sobre un gen.  

En cada línea de un archivo GFF3 se describe una característica genética, siendo cada columna una descripción. La primera columna es el **seqid**, nombre de la secuencia donde se encuentra el feature - referencia principal. Luego viene la fuente (**source**) que habla de la fuente que produjo este gen, entonces si se encontró en GeneBank por ejemplo, se escribirá ese software en ese sector. La tercera columna, **type**, clasifica qué tipo de elemento es lo que estamos analizando— un gen, un exón, un CDS, una región, etc. Las columnas cuatro y cinco, **start y end**, nos marcan las coordenadas donde inicia y termina dicha característica dentro de la secuencia. La columna siguiente es **score**, que expresa la confianza de que ese "feature" existe en esa posición de la secuencia; si no se conoce, se deja como punto (.). En la columna siete, **strand**, se indica si el feature está en la hebra directa (+) o complementaria (-). La columna **phase** se utiliza para los CDS (coding sequence), indicando el marco de lectura para la traducción de codones. Finalmente, la columna número 10, **attributes**, guarda los detalles de lo que se está describiendo: identificadores únicos, nombres de genes, relaciones jerárquicas (como Parent=transcript1), etc.

Ejemplo:
seqid: chr1  source: GenBank   type: gene  start: 1000  end: 5000  score: .  strand: +  phase: .  attributes: ID=gene0001;Name=Oxidasa


## Descripción de especie Apteryx haastii: Kiwi moteado mayor
Según Data Zone (2024) Esta ave es la especie más grabnde de kiwi y es nativa de Nueva Zelanda. Vive en montañas boscosas y se alimenta de invertebrados, frutas caídas y diferentes hojas en el suelo. Su reproducción está basada en la puesta de un huevo e incubarlo por alrededor de 75 - 85 días (de los periodos de incubación más largos entre las aves). Estas aves no son migratorias y tienden a vivir al rededor de 11.5 años, si no mueren antes pues 94% de los polluelos no llegan a la madurez. 

## Sección 3:
**i. ¿Cuantos features contiene el archivo?**
870888

**ii. ¿Cuantas regiones de la secuencia (cromosomas) contiene el archivo?**
4183

**iii. ¿Cuántos genes están listados en el organismo?**
19261  
**Otra manera de hacerlo:**  
16674 gene  
   2537 ncRNA_gene  
     50 pseudogene  
**Donde el total tambien es 19261**  
**Pequeña explicación:**   
**Gene:**  Contienen las instrucciones necesarias para fabricar proteínas que ejecutan funciones en las células.  
**ncARN (Gen de ARN no codificante):** Genes que no generan proteínas, pero sí ARN funcional con roles estratégicos, como regular otros genes o ensamblar estructuras celulares.  
**Pseudogén:** Copias antiguas y no funcionales de genes activos, que ya no producen proteínas.  

**iv. ¿Cuál es el top 10 de tipo de features (columna 3) más anotados en el genoma?**
 1. 337842 exon
 2. 329455 CDS
 3. 135966 biological_region
 4. 27823 mRNA
 5. 16674 gene
 6. 8251 five_prime_UTR
 7. 5247 three_prime_UTR
 8. 4183 region
 9. 2537 ncRNA_gene
 10. 2193 lnc_RNA

## Referencias
Great Spotted Kiwi Apteryx Haastii Species Factsheet | BirdLife DataZone. (2024). BirdLife DataZone. https://datazone.birdlife.org/species/factsheet/great-spotted-kiwi-apteryx-haastii
