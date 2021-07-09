# Recursos externos

Este directorio contiene aquellos elementos (binarios, instaladores, módulos, AMS, plantillas de configuración opcionales ) que o bien son obligatorios y deben ser provistos por el implantador antes de la ejecución de la receta o bien son opcionales y específicos de cada instalación.

## Módulos JAR y AMP

En la carpeta de "addons" se pueden dejar los AMP y los JAR que se desean instalar. La estructura de carpetas esta organizada de tal forma que dependiendo de si es un JAR o un AMP, si es para Share o para el backend/platform/alfresco quede claro donde hay que dejar cada cosa.

## Ficheros mínimos a añadir

A continuación se listan una serie de ficheros que obligatoriamente deben ser provisionados en la carpeta de recursos externos antes de ejecutar la receta. En su defecto la receta fallará.

**Atención desarrolladores!!!** Es importante mantener esta lista actualizada

- installers/alfresco-search-services-1.4.3.4.zip

Descargar de <https://artifacts.alfresco.com/nexus/service/local/repo_groups/public/content/org/alfresco/alfresco-search-services/1.4.3.4/alfresco-search-services-1.4.3.4.zip>
