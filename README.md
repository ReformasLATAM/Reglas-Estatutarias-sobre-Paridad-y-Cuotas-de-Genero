# Reglas Estatutarias sobre Paridad y Cuotas de Género en los Órganos de Dirección Nacionales de los Partidos Políticos Latinoamericanos 

Bienvenidos/as al repositorio GitHub de la base de datos "Reglas Estatutarias sobre Paridad y Cuotas de Genero en los Organos de Direccion Nacionales de los Partidos Politicos Latinoamericanos" mantenida por integrantes del Observatorio de Reformas Políticas en América Latina.

## Contenidos

-   [Resumen](#resumen)
-   [Descripción](#descripción)
-   [Citado](#citado)

## Resumen

La base de datos contiene información descriptiva para conocer la manera en que los partidos políticos en América Latina regulan actualmente la participación de mujeres en la integración de sus órganos de dirección nacionales específicamente en Asambleas, Consejos Políticos y Comités Ejecutivos.

La recolección de información se realizó mediante la consulta de los estatutos de una muestra de 54 partidos políticos en América Latina. Se revisaron las reglas estatutarias sobre paridad y cuotas de género en los órganos de dirección nacionales de las organizaciones partidistas. 

La selección de los partidos que son considerados como relevantes en 18 países de América Latina y que forman parte de las unidades de observación de la base de datos, tiene como antecedente la empleada para la investigación de Alcántara Sáez y Freidenberg (2001), quienes crearon una matriz de selección basada en cuatro criterios: que un partido a) hubiera obtenido representación en la Cámara baja en las tres últimas elecciones legislativas (fuerza numérica expresada en escaños o en votos obtenidos); b) que hubiera superado la barrera del 5% electoral en las tres últimas elecciones legislativas en la Cámara baja; c) que tuviera representación en todos los distritos electorales del país (fuerza territorial) o que su representación en determinados distritos fuera claramente significativa; y d) que contara sustantivamente en la dinámica partidaria del sistema político, es decir, que ejerciera capacidad de influencia en el sistema político (aun cuando no cumpliera las anteriores).

Integrantes del Observatorio de Reformas Políticas en América Latina recopilaron y codificaron la información. Las personas responsables de la recopilación de los datos son Flavia Freidenberg (Instituto de Investigaciones Jurídicas, UNAM) y Carlos Guadarrama (Facultad Latinoamericana de Ciencias Sociales, sede México), mientras que las personas responsables de la codificación de los datos son Flavia Freidenberg (Instituto de Investigaciones Jurídicas, UNAM), Carlos Guadarrama (Facultad Latinoamericana de Ciencias Sociales, sede México) y Karla Estrada (Facultad de Estudios Superiores Acatlán, UNAM). 

## Descripción

El directorio `./Data/` contiene el archivo `./Data/DD_Paridad` en el cual se encuentra toda la información relevante respecto a la base de datos de reglas estatutarias sobre paridad y cuotas de género en los órganos de dirección nacionales de los partidos políticos latinoamericanos. En específico, la base de datos se compone de las siguientes variables:

-   `id_partido`: clave numérica para identificar a cada uno de los 54 partidos políticos en la base de datos. El número a identificar se compone del número del país y el número del partido en la muestra por país.

-   `siglas_partido`: siglas de los nombres de cada uno de los 54 partidos políticos en la base de datos, de acuerdo con fuentes documentales de los propios partidos políticos.

-   `país`: nombre del país al que pertenece el partido político del que se seleccionaron los estatutos en donde se establecen las normas internas respecto a la paridad y cuotas de género en los órganos de dirección nacionales.

-   `cowcode`: código del país de acuerdo con la codificación de “Correlates of War”.
https://correlatesofwar.org/data-sets/cow-country-codes.

-   `siglas_pais`: siglas del país de acuerdo con el código de tres letras ISO (por ejemplo: ARG, MEX, SAL) http://utils.mucattu.com/iso_3166-1.html

-   `año_estatuto`: año de publicación de los estatutos de los partidos políticos entre 1996 y 2020, en los cuales se consultaron las reglas internas sobre paridad y cuotas en los órganos de dirección nacionales. En caso de que la información no esté disponible se usa el número -9999.

-   `paridad`: registra la presencia o ausencia de normas estatutarias en los partidos políticos que estipulen la paridad de género en sus direcciones nacionales. Valores: No [0]: los estatutos de los partidos no contienen reglas que establezcan la paridad de género como criterio para la integración de los órganos de dirección nacional. Sí [1]: los estatutos de los partidos contienen reglas que establezcan la paridad de género como criterio para la integración de los órganos de dirección nacional.

-   `cuota`: registra la presencia o ausencia de normas estatutarias en los partidos políticos que estipulen cuotas de género en la integración de sus direcciones nacionales. Valores: No [0]: los estatutos de los partidos no contienen reglas que establezcan cuotas de género como criterio para la integración de los órganos de dirección nacional. Sí [1]: los estatutos de los partidos contienen reglas que establezcan cuotas de género como criterio para la integración de los órganos de dirección nacional.

-   `porcentaje`: indica el porcentaje que los estatutos de los partidos políticos establecen para las cuotas de género. Valores: 888: en caso de que los estatutos estipulen cuotas de género, pero no establezcan una cifra para ellas. 999: en caso de que los estatutos no precisen cifras para las cuotas de género.

-   `organos_direccion`: indica si el carácter de los órganos de dirección a los cuáles se aplican las normas de paridad y cuotas de género de los estatutos de los partidos políticos es específico o general para todos los órganos de dirección. Valores: Órganos específicos [1]: En las reglas estatutarias de paridad y cuotas de género se señalan expresamente los órganos de dirección a los cuales se aplican estos criterios en su integración. Todos los órganos [2]: En las reglas estatutarias de paridad y cuotas de género no se establece distinción entre los órganos de dirección a los cuales se aplican estos criterios en su integración. No se determina [99]: En las reglas estatutarias de paridad y cuotas de género no se estipula a cuáles órganos de dirección se aplican estos criterios en su integración.

-   `organo_n`: indica cuáles son los órganos específicos de dirección de los partidos políticos a los que se aplican las reglas sobre paridad y cuotas de género establecidas en sus estatutos.
Valores: Asamblea [1]: Los estatutos de los partidos políticos establecen como uno de los órganos de dirección a los cuales se aplican las reglas de paridad y cuotas a las Asambleas Nacionales o su equivalente. Consejo Político Nacional [2]: Los estatutos de los partidos políticos establecen como uno de los órganos de dirección a los cuales se aplican las reglas de paridad y cuotas a los Consejos Políticos Nacionales o su equivalente.Comité Ejecutivo Nacional [3]: Los estatutos de los partidos políticos establecen como uno de los órganos de dirección a los cuales se aplican las reglas de paridad y cuotas a los Comités Ejecutivos Nacionales o su equivalente.

-   `art_n`: indica el número del artículo en los estatutos de los partidos políticos donde se establecen las normas de paridad y cuotas de género.

## Citado

``` r
Observatorio de Reformas Políticas en América Latina (1978-2023). Tabla Comparativa “Reglas estatutarias sobre paridad y cuotas de género en los órganos de dirección nacionales de los partidos políticos latinoamericanos”, Ciudad de México: Instituto de Investigaciones Jurídicas (IIJUNAM) y Washington, D.C.: Secretaría para el Fortalecimiento de la Democracia de la Organización de los Estados Americanos (SFD/OEA). Disponible en: https://doi.org/10.6084/m9.figshare.14535651.v2.
```