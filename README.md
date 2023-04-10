# Proyecto final de analisis y sistemas
### Francisco Ogando (2021-0160)
[Link a la explicación de la app](https://miucateciedu-my.sharepoint.com/personal/20210160_miucateci_edu_do/_layouts/15/onedrive.aspx?login_hint=20210160%40miucateci%2Eedu%2Edo&id=%2Fpersonal%2F20210160%5Fmiucateci%5Fedu%5Fdo%2FDocuments%2FAn%C3%A1lisis%20de%20sist%2Fdocker%2Dcompose%2Eyml%20%2D%20APP%20%2D%20Visual%20Studio%20Code%202023%2D04%2D10%2014%2D53%2D02%2Emp4&parent=%2Fpersonal%2F20210160%5Fmiucateci%5Fedu%5Fdo%2FDocuments%2FAn%C3%A1lisis%20de%20sist)



***Para entender cómo funciona la aplicación, analizamos detalladamente las carpetas de client, worker, nginx y server, así como el archivo Docker Compose, sabiendo que necesario comprender primero el propósito de cada una de estas carpetas y cómo se relacionan entre sí.***

***La carpeta "client" contiene los archivos necesarios para crear la interfaz de usuario de la aplicación. Estos archivos pueden incluir HTML, CSS, JavaScript y cualquier otro recurso necesario para crear la experiencia del usuario final.***

***La carpeta "worker" contiene los archivos necesarios para procesar tareas en segundo plano en la aplicación. Esto puede incluir procesamiento de datos, envío de correos electrónicos o cualquier otro proceso que deba ejecutarse fuera del proceso principal de la aplicación.***

***La carpeta "nginx" contiene los archivos necesarios para configurar un servidor web Nginx que actúa como proxy inverso para la aplicación. El proxy inverso se encarga de recibir todas las solicitudes del cliente y dirigirlas al servidor adecuado para su procesamiento. También puede manejar la caché y la seguridad de la aplicación.***

***La carpeta "server" contiene los archivos necesarios para crear el servidor principal de la aplicación. Esto incluye código fuente, dependencias y cualquier otro recurso necesario para ejecutar la aplicación.***

***Docker Compose es una herramienta que permite a los desarrolladores definir y ejecutar aplicaciones Docker de múltiples contenedores. Un archivo Docker Compose define cómo se ejecutan los contenedores de la aplicación y cómo se comunican entre sí.***

**En el contexto de esta aplicación, un archivo Docker Compose podría definir los siguientes contenedores:**
<p> 
Un contenedor para la aplicación del servidor, que incluiría la carpeta "server" y cualquier dependencia necesaria para ejecutar la aplicación.
<p/>
<p>
Un contenedor para la interfaz de usuario de la aplicación, que incluiría la carpeta "client" y cualquier recurso necesario para construir la interfaz de usuario.
<p/>
<p>
Un contenedor para el procesamiento en segundo plano, que incluiría la carpeta "worker" y cualquier recurso necesario para procesar tareas en segundo plano.
<p/>
<p>
Un contenedor para el servidor Nginx, que incluiría la carpeta "nginx" y cualquier configuración necesaria para actuar como proxy inverso para la aplicación.
<p/>

***Cada contenedor estaría aislado de los demás y solo tendría acceso a los recursos que se le asignan. El archivo Docker Compose definiría cómo se comunican los contenedores entre sí y cómo se exponen los puertos de los contenedores a través de la red.***

***En resumen, la aplicación se ejecuta en múltiples contenedores Docker aislados, cada uno con su propia función específica. Docker Compose se encarga de definir y orquestar la ejecución de estos contenedores y de gestionar la comunicación entre ellos.***