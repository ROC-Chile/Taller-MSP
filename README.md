# Taller: Fortalecimiento del capital humano y herramientas analíticas en torno al monitoreo de aves playeras en Chile

El Migratory Shorebird Project(MSP) busca potenciar las capacidades locales para soluciones en la conservación de humedales a lo largo de la costa Pacifica de las Américas. Una arista del MSP se enfoca en el uso de los datos recolectados por censos estandarizados en sitios de importancia para aves playeras. En ese contexto, este repositorio busca entregar una herramienta analítica que describe el procedimiento para obtener tendencias en abundancia a nivel de especies, sitios y nacional de aves playeras, utilizando datos esquema de monitoreo (1) [MSP](https://migratoryshorebirdproject.org/), (2) [CNAA](https://lac.wetlands.org/nuestro-enfoque/humedales-y-naturaleza-saludables/censo-neotropical-de-aves-acuaticas/) (Censo Neotropical de Aves Acuáticas) y (3) [CCAP](https://whsrn.org/wp-content/uploads/2019/05/coastalshorebirdsurvey_manual_latam_spanish.pdf) (Censo Costero de Aves Playeras). Hemos desarrollado un ejemplo ilustrativo con datos de estos esquemas recolectados en Chile. No obstante, este código busca ser facilmente adaptable para datos recolectado bajo estos esquema en cualquier país involucrado.

El código está estructurado como un tutorial, detallando los pasos a seguir utilizando el paquete **SpAbundance** de [Doser et al. 2024](https://besjournals.onlinelibrary.wiley.com/doi/pdf/10.1111/2041-210X.14332). Este paquete trabaja en un marco de estadística Bayesiana, pero drásticamente simplifica su implementación al adoptar el syntax ampliamente utilizado por paquetes como **lmer**. El uso de esta herramienta requiere un conocimiento moderado de R.

## Cómo utilizar el código
Empezar por el archivo [Taller.Rmd](https://github.com/ROC-Chile/Taller-MSP/blob/main/Taller.Rmd) que contiene el código para preparar los datos de mutilples esquemas de monitoreo (en este caso tres), integra los datos y realiza un modelo generalizado mixto Bayesiano para determinar abundancia y tendencias en el tiempo y grafica los resultados. 

## 
Si tienes preguntas puedes contactarte con nosotros enviando un correo a [Marion Díaz](mariondiaz@redobservadores.cl) o [Erik Sandvig](eriksandvig@redobservadores.cl) del Programa de Monitoreo de la ROC.

Este tutorial fue desarrollado por la [Red de Observadores de Aves y Vida Silvestre de Chile (ROC)](https://www.redobservadores.cl) en el marco de un proyecto [MSP+](https://msp-plus.pointblue.org/es/) otorgado por [Point Blue Conservation](https://www.pointblue.org).
