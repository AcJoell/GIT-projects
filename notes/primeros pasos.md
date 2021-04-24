_________________________________

<h1> CREANDO UN REPOSITORIO </h1>
_________________________________

<h2>COMANDOS:</h2>

<p>
NOTA:
- usas letras (l, a)
-- usas palabras (global)
</p>

<h3>git config || git config --list || git config --list --show --origin</h3>

<p>
Encontraras todas las configuraciones de git
--list veras la configuracion por defecto de tu git y las cosas que te faltan
--list --show --origin muestra donde se encuentran las configuraciones guardadas
</p>

<h3>git config --global user.name "Your Name"</h3>

<p>
Configura tu nombre para que cualquier colaborador o tu lo puedan ver
</p>

<h3>git config --global user.email "user@example.com"</h3>

<p>
Configura tu correo
</p>
_________________________________

<h1> CREANDO UN REPOSITORIO </h1>
_________________________________

<h2>COMANDOS:</h2>

<h3>git init</h3>

<p>
Se inicia el repositorio vacio
</p>

<h3>git add .</h3>

<p>
Agregamos todos los archivos nuevos o alterados
</p>

<h3>git rm name.txt</h3>

<p>
Sacar un archivo el cual agregaste (mediante git add)
</p>

<h3>git rm --cached name.txt</h3>

<p>
Se quita el add del archivo, cuando ponemos el cached significa que esta en RAM, aun no se ha guardado en la DB
</p>

_________________________________

<h1> HACIENDO TU PRIMET COMMIT </h1>
_________________________________

<h2>COMANDOS:</h2>

<p>
NOTA:
si hiciste commit y alteraste un archivo que quieres guardar u hiciste otra accion tienes que repetir el proceso haciendo:
git add .
git commit -m "Newmessage"
</p>

<h3>git commit -m "message"</h3>

<p>
Te envia el mensaje escrito dentro de las comillas a la hora de guardar los cambios en el repositorio remoto
</p>

<h3>git diff numLargoDelCommit1 numLargoDelCommit2</h3>

<p>
Sirve para comparar los cambios hechos entre commits
</p>

