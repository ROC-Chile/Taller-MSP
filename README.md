# Taller: Fortalecimiento del capital humano y herramientas analíticas en torno al monitoreo de aves playeras en Chile

El Migratory Shorebird Project(MSP) busca potenciar las capacidades locales para soluciones en la conservación de humedales a lo largo de la costa Pacifica de las Américas. Una arista del MSP se enfoca en el uso de los datos recolectados por censos estandarizados en sitios de importancia para aves playeras. En ese contexto, este repositorio busca entregar una herramienta analítica abierta que describe el procedimiento para estimar abundancias y tendencias a nivel de especies y sitios de aves playeras, utilizando datos de los esquemas de monitoreo (1) [MSP](https://migratoryshorebirdproject.org/), (2) [CNAA](https://lac.wetlands.org/nuestro-enfoque/humedales-y-naturaleza-saludables/censo-neotropical-de-aves-acuaticas/) (Censo Neotropical de Aves Acuáticas) y (3) [CCAP](https://whsrn.org/wp-content/uploads/2019/05/coastalshorebirdsurvey_manual_latam_spanish.pdf) (Censo Costero de Aves Playeras). Este repositorio consta de un ejemplo ilustrativo utilizando los datos de estos tres esquemas en Chile. No obstante, este código es facilmente adaptable para datos recolectado bajo estos esquema en cualquier país involucrado. Esperamos que organizaciones e investigadores en otros países puedan hacer uso de este modelo para sus datos.

El código está estructurado como un tutorial, detallando los pasos a seguir para preparar los datos (utilizamos como ejemplo la preparación de datos MSP) y construir el modelo utilizando el paquete **SpAbundance** de [Doser et al. 2024](https://besjournals.onlinelibrary.wiley.com/doi/pdf/10.1111/2041-210X.14332). Este paquete permite construir modelos bajo un marco de estadística Bayesiana, pero drásticamente simplifica su implementación al adoptar el syntax ampliamente utilizado por paquetes ampliamente utilizados como **lmer**. El modelo desarrollado como ejemplo es simple, pero permite la inclusión sencilla de variables adicionales que puedan ser de su interés. Para aprovechar al máxima esta herramienta se requiere un conocimiento moderado de R.

## Cómo utilizar el código
En el archivo [Taller.Rmd](https://github.com/ROC-Chile/Taller-MSP/blob/main/Taller.Rmd) encontrarán el código. Sigue la siguiente estructura:
1. Preparar los datos en el formato requerido por [spAbundance](https://doserlab.com/files/spabundance-web/) e integra los datos de los distintos esquemas en una sola base de datos.
2. Construye un Modelo Lineal Generalizado Mixto (GLMM) para determinar abundancia y tendencias en el tiempo.
3. Grafica los resultados del modelo con ejemplos a nivel de especie, sitio y total entre sitios. 

## 
Si tienes preguntas o necesitas ayuda para usar este código puedes enviar un correo a [Marion Díaz](mariondiaz@redobservadores.cl) o [Erik Sandvig](eriksandvig@redobservadores.cl).

Este tutorial fue desarrollado por el Programa de Monitoreo de Aves de la [Red de Observadores de Aves y Vida Silvestre de Chile (ROC)](https://www.redobservadores.cl) gracias al financiamiento del programa [MSP+](https://msp-plus.pointblue.org/es/) de [Point Blue Conservation](https://www.pointblue.org).
