# Versiones de SIGMA Automatizador - Informe Conclusivo

Este repositorio público contiene únicamente el manifiesto `version.json` que
consulta la aplicación al iniciarse. No contiene código fuente, credenciales ni
documentación de las auditorías.

## Dirección pública utilizada por la aplicación

`https://raw.githubusercontent.com/federicoderodrigo/sigma-automatizador-informe-conclusivo-versiones/main/version.json`

## Procedimiento para publicar una actualización

1. Compilar, probar y cerrar la nueva versión de la aplicación.
2. Preparar la carpeta completa y su ZIP con el número de versión en el nombre.
3. Subir una nueva versión del mismo archivo ZIP de Google Drive, conservando
   su ID, enlace y permisos. Actualizar el nombre visible y comprobar la carga.
4. Actualizar `latestVersion` en `version.json` solamente cuando la descarga ya
   esté disponible.
5. Mantener `mandatory` en `true`. La aplicación bloquea las versiones anteriores
   a `latestVersion`; admite la misma versión y las superiores de prueba local.
6. Completar `downloadUrl` con el enlace público o institucional de Google Drive
   cuando esté disponible.
7. Publicar en `sha256` la huella SHA-256 del ZIP para poder comprobar que la
   copia descargada es exactamente la distribución oficial.

Si GitHub no puede consultarse, la aplicación muestra un error y permite volver
a intentar o cerrar. Esta decisión asegura que no se trabaje sin conocer la
versión oficial vigente.
