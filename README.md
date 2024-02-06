1) Esta trabajando en un proyecto Git colaborativo con varias ramas y commits. Tu tarea es utilizar el comando git log con algunas opciones específicas para obtener un resumen gráfico de los últimos 5 commits en todas las ramas.

<img src="/images/alias 1.png">

2) Esta trabajando en un proyecto Git colaborativo y necesitas obtener una visión gráfica y
   detallada del historial de commits. Tu tarea es utilizar el comando git log con opciones
   específicas para personalizar el formato y presentación de la salida. La salida debe tener
   las siguientes especificaciones:

*Muestra una representación gráfica del historial de commits

*Muestra el hash corto del commit en color rojo

*Muestra las referencias (ramas o tags) en las que está involucrado el commit en color
amarillo

*Muestra el mensaje del commit.

*Muestra la fecha relativa del commit en color verde.

*Muestra el hash del commit como un identificador abreviado.

*Muestra las fechas de los commits de forma relativa

![image-20240205165754196](C:\Users\ANTONIO JOSE\AppData\Roaming\Typora\typora-user-images\image-20240205165754196.png)

3) Estas trabajas frecuentemente con el comando git log -1 HEAD para obtener detalles sobre
   el último commit en la rama actual. Sin embargo, encuentras que escribir este comando
   completo es un poco tedioso. Quieres simplificarlo creando un alias personalizado.

   Tu tarea es utilizar el comando git config para crear un alias llamado last que represente el
   comando git log -1 HEAD.

![image-20240205170424672](C:\Users\ANTONIO JOSE\AppData\Roaming\Typora\typora-user-images\image-20240205170424672.png)

4) Imagina que deseas simplificar el proceso de editar la configuración global de Git. Tu tarea
   es utilizar el comando git config para crear un alias que te permita abrir fácilmente la
   configuración global en tu editor de texto preferido. Ejecuta el comando para crear un alias
   llamado ec que cumpla con la especificación dada.

![image-20240205172406089](C:\Users\ANTONIO JOSE\AppData\Roaming\Typora\typora-user-images\image-20240205172406089.png)

5) Imagina que estás trabajando en un proyecto Git colaborativo con múltiples colaboradores
   y ramas. Tu tarea es utilizar el comando git log con opciones específicas para personalizar
   la salida del historial de commits y resaltar información clave.

![image-20240205182039163](C:\Users\ANTONIO JOSE\AppData\Roaming\Typora\typora-user-images\image-20240205182039163.png)

ALIAS USADOS EN ESTA ACTIVIDAD

[alias]

Estrutura utilizada para configurar alias: **git config --global alias.NombreAlias "comando a convertir"**

Ejemplo: **git config --global alias.last "log -1 HEAD"**

1.  **lg = log --graph --abbrev-commit --decorate --format=format:'%C(bold\nred)%h%C(reset) - %C(bold green) 	 (%ar)%C(reset)%C(white)%s%C(reset)%C(dim\nwhite)-%an%C(reset)%C(bold yellow)%d%C(reset)' --all**

​	%C(color): Esta secuencia de formato permite especificar el color del texto que le sigue. Por ejemplo, 			   %C(red) establece el color rojo.

​	%h: Muestra el hash corto del commit.

​	 %s: Muestra el mensaje del commit.

​	 %an: Muestra el nombre del autor del commit.

​	 %d: Si un commit está referenciado por una rama o una etiqueta, `%d` se usa para mostrar esas 		 referencias.

​	  %ar: Muestra la fecha relativa del commit en un formato legible para humanos, como "hace 2 horas"  		   o "hace 3 días". Es útil para tener una idea rápida de cuándo se realizó un commit en relación 		   con el tiempo actual.

2. **last = log -1 HEAD** - Muestra el último commit del HEAD actual del repositorio.

3. **ec = config --global -e**  - Abre el archivo de configuración global de Git en el editor de texto configurado en tu sistema

4. **graph = log --oneline --decorate --all --graph** - Muestra un registro de commits en una sola línea, con información adicional como las ramas y etiquetas que apuntan a cada commit, y una representación gráfica de la historia del repositorio.

5. **outp = log --pretty=format:'%C(bold yellow)%h%Creset%C(red)\\%d %C(white)%s%Creset%C(blue)\\ [%an]'**

   Proporciona un formato de salida personalizado



