Ajustes Visual Studio para biblioteca de audio:


Para la configuración dentro de Visual, abrimos las propiedades del proyecto, seleccionamos
Directorios de VC++, y luego en Directorios de archivos de inclusión, y se pega la siguiente
línea:

$(SolutionDir)\Externals\includes;$(IncludePath) 

Ahora vamos a Vinculador/Entrada/Dependencias adicionales, y pegamos el texto:
irrKlang.lib

Damos aplicar, y estará listo para usar Irrklang en el código.


------------------------------------ IMPORTANTE -------------------------------------
Si al momento de ejecutar el proyecto aparecen errores de compilacion es probable que
se estén ocupando herramientas de compilación que no están instaladas en la version de
Visual Studio que se está utilizando. 

Si este es el caso, dentro de Visual Studio favor de hacer lo siguiente:

1.- Seleccionar el menú Proyecto.
2.- Seleccionar la opción de Propiedades de Proyecto.
3.- Ir a la opción General.
4.- En la opción que dice "Conjunto de herramientas de la plataforma" seleccionar la version de
    herramientas de compilación que se tengan instaladas.
5.- Dar clic en la opción Aceptar.
6.- Por último volver a ejecutar el código para verificar que el error desaparece.


