# PracticaWebDbZap
Práctica del uso de Zap, para aprender a detectar vulnerabilidades de un sistema

--------------------------------------------------------------------------------

Checklist para entregar (pegar en el repo README)
- Código fuente completo y ejecutable.
- Capturas ZAP: Sites, Alerts list, Alert detail.
- Reporte (PDF) con comparativa antes/después.
- package.json y seed.sql incluidos.
- Instrucciones de ejecución (README).

--------------------------------------------------------------------------------
INSTRUCCIONES DE EJECUCIÓN

Instalaciones
- Instalación de ZAP y navegador Mozilla Firefox
  
Configuración de ZAP en el navegador
- Abrir ZAP
- En cualquier navegador, busca el sitio http://localhost:8080
- Descargar el certificado de ZAP
- Abrir el navegador Firefox
    Configuración conexión
    - En configuración, en el panel General, desplazarse hasta abajo y buscar la sección Configuración de conexión
    - Dar clic en Configurar.
    - Seleccionar opción de Configuración manual de proxy.
    - En Proxy HTTP agregar la dirección 127.0.0.1 y el puerto 8080
    Configuración de certificado ZAP
    - En el panel Privacidad y seguridad, buscar la sección de certificados.
    - Dar clic en Ver certificados
    - Dar clic en Importar y seleccionar el certificado de ZAP descargado anteriormente.
    - Dar clic en Aceptar
    
Configuración de ZAP
- Abrir ZAP
- Irse al panel de Herramientas
- Dar clic en Opciones
- Irse a la sección de Selenium
- Buscar el apartado de Binarios - Firefox
- En el campo de Binario, elegir la ruta donde se encuentre firefox.exe
- En el campo de Perfil por defecto, elegir zap-client-profile
- Dar clic en aceptar
 
Ejecución de programa 
- En consola, dirigirse a la ubicación de la carpeta del proyecto
    Ej.
    cd C:\Proyectos\PracticaWebDbZap\zap-labVulnerable
- Escribir node app.js

Ejecución de pruebas de seguridad en ZAP
- Dar clic en Exploración Manual
- En el campo URL a explorar poner http://localhost:3000.
- Habilitar e campo Habilitar el HUD
- Dar clic en Iniciar navegador
- Abierto el navegador, explorar todas las opciones de la página
- En ZAP, explorar el panel Historial, Alertas, etc.
