Ajustes Visual Studio para biblioteca de audio:


Para la configuración dentro de Visual, abrimos las propiedades del proyecto, seleccionamos
Directorios de VC++, y luego en Directorios de archivos de inclusión, y se pega la siguiente
línea:

$(SolutionDir)\Externals\includes;$(IncludePath) 

Ahora vamos a Vinculador/Entrada/Dependencias adicionales, y pegamos el texto:
irrKlang.lib

Damos aplicar, y estará listo para usar Irrklang en el código.

