# Proyecto-malla-universidad

*Descripcion del proyecto

- En este proyecto se busca implementar el desarrollo de una aplicación web full-stack orientada a la visualización interactiva de las mallas curriculares de las carreras impartidas por la Universidad Mayor. La solución busca facilitar el acceso y comprensión de la estructura académica por parte de los estudiantes.
- La plataforma permite explorar de manera dinámica las asignaturas organizadas por semestre, conocer sus prerrequisitos, electivos, certificaciones. Al ofrecer una interfaz intuitiva y centralizar la información académica, se espera mejorar significativamente la experiencia de planificación académica, reducir errores en la toma de decisiones y fomentar una mayor autonomía de los estudiantes.
- Esta aplicación también representa una oportunidad para digitalizar procesos que tradicionalmente se basan en documentos estáticos (como PDF), promoviendo la transformación digital dentro del ámbito universitario.

*Justificación Tecnológicas
- Front-End: Se optó por una solución con el uso de HTML, CSS, JavaScript. Esta elección responde a la necesidad de mantener una estructura ligera, de fácil mantenimiento y sin dependencias externas y a su vez  para un prototipo funcional y navegable.

- Backend: Se utilizó Node.js con el framework Express.js, para construir el servidor y aplicar API RES, proporcionado una estructura mínima pero poderosa para definir rutas, manejar peticiones HTTP, facilitando la integración con el Front-End y la base de datos. 

- Base de Datos: Se decidió usar PostgreSQL por su robusta, escalable y su código abierto, que permite modelar eficientemente relaciones entre entidades como carreras, asignaturas, prerrequisitos y certificaciones.

*Manual de Entorno e Instalación

- Este manual está diseñado para cualquier persona externa al equipo de desarrollo que desee ejecutar localmente el proyecto de malla curricular interactiva, sin necesidad de conocimientos técnicos avanzados o experiencia previa.
Requisitos previos:
1) Se debe descargar e instalar los siguiente:
   
- Node.js (v18 o superior)
- Visual Studio Code
- Git (opcional)
- Un navegador cualquiera (Google, Opera, entre otros)
  
2) Descargar el proyecto:
  
Opción A: Clonar desde GitHub: 

a) Primero deberá tener instalado Git.
b) Acceda a Visual Studio Code.
c) Busque dónde está la ventana de Terminal, elija nuevo terminal.
d) Escriba lo siguiente en el terminal:
git clone https://github.com/Matador2222/Malla-curricular.git
git clone https://github.com/Matador2222/back-end-malla-universidad.git

Opción B: descargarla desde GitHub:

a) Acceda al repositorio de proyecto: https://github.com/Matador2222/Malla-curricular
https://github.com/Matador2222/back-end-malla-universidad
b) Vaya al botón verde donde dice: Code, y seleccione “Download ZIP”.
c) Extraiga el contenido en su computador.

3) Configuración del backend
 
a) En el Visual Studio Code, vaya a la ventana de Archivo y seleccione Abrir Archivo… y busque Back-End Malla Universidad.
b) Acceder al terminal y escriba lo siguiente: 
npm install
c) Vaya a la ventana de Archivo y seleccione Nuevo Archivo…
d) Crea el archivo llamado .env, en la raíz del backend .
e) En la carpeta .env recientemente creada, agregue la siguiente línea de código:
DATABASE_URL=postgres://usuario:clave@host:puerto/nombre_bd
- Este es un ejemplo demostrativo. La URL real de conexión será entregada por el equipo administrador del proyecto o estará disponible en la plataforma Railway.

3A) Error al usar npm install

a) Busque PowerShell en el menú de inicio.
b) Seleccione como administrador.
c) Escriba el siguiente comando:
Set-ExecutionPolicy
d) Luego escriba “S” para confirmar.
e) Cierre el Visual Studio Code y ejecutalo de nuevo.
f) Vuelva a utilizar el comando npm install en la terminal.

4) Ejecucion del servidor
   
a) Vaya a un terminal y escriba:
node app.js.
b) El backend quedará activo en http://localhost:3000.
c) y se conectará automáticamente a la base de datos en Railway.

5) Visualización de la aplicación web

a) Diríjase a la carpeta: Malla_Universida_Mayor.
b) Abra el archivo index.html.
La aplicación debería cargar automáticamente los datos desde el backend conectado a Railway.
