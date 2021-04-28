_________________________________

<h1> INTRODUCCION A RAMAS </h1>
_________________________________

<h2>COMANDOS:</h2>

<h3>MASTER</h3>

<p>
MASTER es la rama por defecto
</p>

<h3>RAMA EXPERIMENTAL O DEVELOPMENT</h3>

<p>
Puedes hacer diferentes cambios sin perjudicar la rama por defecto MASTER
</p>

<h3>RAMA BUGFIXING O HOTFIX</h3>

<p>
Haces los cambios en esa rama y luego los pruabas con la rama actual (MASTER) esa conexion se le conoce como MERGE donde unes los cambios de una rama con otra.
</p>

_________________________________

<h1> VOLVER A UN COMMIT VIEJO </h1>
_________________________________

<h2>COMANDOS:</h2>

<h3>git commit -m "message"</h3>

<p>
Te envia el mensaje escrito dentro de las comillas a la hora de guardar los cambios en el repositorio remoto
</p>

<h3>git reset || git reset --hard  || git reset --soft</h3>

<p>
Nos permite volver a un commit anterior
--hard es el mas peligroso pero el que mas se usa
--soft volvemos a la version anterior, pero lo que tengamos en staying (add) sigue ahi para el proximo commit aunque vuelva a la version anterior
</p>

<h3>git diff</h3>

<p>
Nos muestra los cambios que no han sido agregados en el staying (add) todavia.
</p>