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
_Opcion 1_
<pre>
git checkout week2
git pull origin master
git push origin week2
git checkout master
git pull origin week2 
</pre>
_Opcion 2_
<pre>
git checkout master
git pull origin master
git merge week2
git push origin master
</pre>
