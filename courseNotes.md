# Data Science ToolBox Course Notes
## Week 2 
### Git and Github

Comandos usados para el curso:

configuración
<pre>
git config --global user.name "Nombre"          #Configurar nombre
git config --global user.email "corre@dom.com"  #Configurar email
git list                                        #Lista la configuración
</pre>

Comandos varios
<pre>
git clone                  # Clonar repo hacia local
git init                   # Indicar que el directorio local se registre en git
git remote add origin https://....git
</pre>

Agregar, comitear y push y pull
<pre>
git add .                              # Agregar archivos creados
git add -u                             # Agregar los modificados
git add -A                             # Agregar los dos casos anteriores
git remote add origin https://....git  # Agregar origen remoto
git commit -m "Mensaje del commit"     # Comit a los locales hacia git
git push                               # Comit a github
git checkout branch                    # Cambiar hacia un branch
</pre>


__Secuencias para sincronizar__
<pre>
git checkout week2
git pull origin master
git push origin week2
git checkout master
git pull origin week2 
</pre>

### R Packaging

Comandos basicos para manejar paquetes desde R. Estas funciones pueden realizarse desde rstudio tambien.
<pre>
install.packages( pkgs= "<name_of_the_package>" )             # Instalar un paquete
update.packages("<Name_of_a_package>")                        # Actualizar
install.packages( pkgs= c("<name_of_the_package>","dos") )    # Instalar un paquete
library("<Name_of_a_package>")                                # Cargar un paquete
require("<Name_of_a_package>")                                # Requerir un paquete
</pre>

Como obtener ayuda
<pre>
help.start()  #Loads an HTML help page in the browser
help( <Name_of_a_package_or_function> )  #Provides documentation for the requested package or function
? <Name_of_a_package_or_function> #Provides documentation for the requested package or function
help.search( "<keyword>" )   #Searches help documents for the <keyword>
?? <keyword>   #Searches help documents for the <keyword>
</pre>
