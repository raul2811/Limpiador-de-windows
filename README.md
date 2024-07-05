# Limpiador-de-windows
Este script de lotes (.bat) está diseñado para eliminar archivos temporales y directorios de tu sistema Windows. Elimina los archivos y directorios temporales del usuario actual y del sistema, así como el contenido de la carpeta Prefetch.
## Contenido del Script

El script realiza las siguientes acciones:

- Elimina todos los archivos en el directorio temporal del usuario actual.
- Elimina el directorio temporal del usuario actual.
- Elimina todos los archivos en el directorio temporal del sistema.
- Elimina el directorio temporal del sistema.
- Elimina todos los archivos en la carpeta Prefetch de Windows.
- Elimina el directorio Prefetch de Windows.
- Cierra la ventana del símbolo del sistema.
### Código del Script
```bat
del C:\Users\%username%\AppData\Local\Temp /f /s /q
rd C:\Users\%username%\AppData\Local\Temp /s /q
del c:\Windows\Temp /f /s /q
rd c:\Windows\Temp /s /q
del C:\Windows\Prefetch /f /s /q
rd C:\Windows\Prefetch /s /q
EXIT
```
## Instrucciones de Uso
- Descarga el archivo Eliminar archivos temp .bat.
- Haz doble clic en el archivo para ejecutarlo.
- Se abrirá una ventana del símbolo del sistema que ejecutará el script y se cerrará automáticamente una vez que termine.

### Notas Importantes
- Permisos de administrador: Este script requiere permisos de administrador para eliminar archivos y directorios del sistema. Asegúrate de ejecutarlo como administrador.
- Precaución: El script elimina permanentemente los archivos y directorios especificados. Asegúrate de que no necesitas recuperar ninguno de los archivos eliminados antes de ejecutar el script.
- 
### Solución de Problemas
- Si el script no se ejecuta correctamente, verifica que tienes permisos de administrador.
- Asegúrate de que las rutas especificadas en el script existen en tu sistema.

## Contribución

Si deseas mejorar este script o agregar nuevas funcionalidades, no dudes en hacer un fork del proyecto y enviar tus cambios mediante un pull request.
