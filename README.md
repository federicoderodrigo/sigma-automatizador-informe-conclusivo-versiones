# Versiones de SIGMA Automatizador - Informe Conclusivo

Este repositorio público contiene únicamente el manifiesto `version.json` que
consulta la aplicación al iniciarse. No contiene código fuente, credenciales ni
documentación de las auditorías.

## Dirección pública utilizada por la aplicación

`https://raw.githubusercontent.com/federicoderodrigo/sigma-automatizador-informe-conclusivo-versiones/main/version.json`

## Procedimiento para publicar una actualización

1. Compilar, probar y cerrar la nueva versión de la aplicación.
2. Preparar la carpeta completa y su ZIP con el número de versión en el nombre.
3. Reemplazar el ZIP oficial dentro de la carpeta compartida de Google Drive.
4. Actualizar `latestVersion` en `version.json` solamente cuando la descarga ya
   esté disponible.
5. Mantener `mandatory` en `true` para impedir el uso de versiones distintas.
6. Completar `downloadUrl` con el enlace público o institucional de Google Drive
   cuando esté disponible.
7. Publicar en `sha256` la huella SHA-256 del ZIP para poder comprobar que la
   copia descargada es exactamente la distribución oficial.

Si GitHub no puede consultarse, la aplicación muestra un error y permite volver
a intentar o cerrar. Esta decisión asegura que no se trabaje sin conocer la
versión oficial vigente.
