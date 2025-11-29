# ProyectoPI1

Primer proyecto de la asignatura PI  

Modificaciones realizadas:  

**Modificación de nombres de usuarios y contraseñas**  

En cada servidor, se han modificado las credenciales de acceso. También se ha modificado las credenciales de acceso a la base de datos de la aplicación `Guestbook`.  

**Instalación de phpMyAdmin**  

En el servidor web se ha instalado esta aplicación y se ha enlazado con el servidor de base de datos, además de crear un usuario con privilegios, `admin`.  
A la aplicación se accederá mediante `http://gestion.base.org/` .  

**Sustitución de apache2 por Nginx + PHP-FPM**  

Se ha desactivado el rol apache2 y se ha creado y activado el rol nginx.  

**Instalacion fail2ban**  

En el servidor web, que va a ser el único accesible desde el exterior, se ha instalado `fail2ban`para controlar el acceso remoto al servidor.  

**Instalación App Biblioteca**  

Se ha instalado la aplicación Biblioteca a la cual se puede acceder mediante `http://biblioteca.dani.org/`.  
Para ello, se han creado dos roles, `biblioteca` que realiza la instalación en el servidor web y `bibliobd` que se encarga de crear un nuevo usuario e importar `biblioteca.sql` en el servidor de base de datos.  
Sin embargo, no he podido pasar de la pantalla de Login. La conexión con la base de datos remota es exitosa y la página carga PHP correctamente, pero no loguea, tampoco devuelve errores.
