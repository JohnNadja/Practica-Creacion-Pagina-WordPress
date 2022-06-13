# Practica para la creacion de una página web de WordPress a través de Azure

## WordPress, ¿qué es?

![wordpress-icon](https://github.com/JohnNadja/Practica-Creacion-Pagina-WordPress/blob/main/images/wordpress-icon.png)

En pocas palabras, ***WordPress*** es un sistema de gestión de contenidos que permite a los usuarios crear páginas web con una interfaz simple y fácil de usar. En ella se pueden crear páginas, publicar contenido, administrar contenido, y mucho más. Además, se puede crear un sitio web con una sola página, o un sitio web con una serie de páginas. 

----
## ¿Cómo crear una página web a través de [Azure](https://azure.microsoft.com/en-us/)?

![azure-icon](https://github.com/JohnNadja/Practica-Creacion-Pagina-WordPress/blob/main/images/microsoft-azure-icon.png)

Antes que nada, se debe tener en cuenta los siguientes aspectos:
- ¿Qué es la [nube](https://azure.microsoft.com/en-us/overview/what-is-the-cloud/)?
- ¿Cómo funciona la nube [Azure](https://docs.microsoft.com/en-us/azure/cloud-adoption-framework/get-started/what-is-azure)?
- ¿Cómo [acceder](https://azure.microsoft.com/es-mx/features/azure-portal/) a Azure?

Si por alguna razón no se está familiarizado con estos aspectos, se pueden consultar en los enlaces que se tienen marcados en las preguntas.

Considerado lo anterior, se procederá a usar un servicio que proporciona el portal de Azure y es **Marketplace**.

---
## Marketplace
![marketplace-icon](https://github.com/JohnNadja/Practica-Creacion-Pagina-WordPress/blob/main/images/store-marketplace.png)

Marquetplace es una plataforma que permite a los usuarios crear sus propias aplicaciones y servicios, desde simples sitios web hasta aplicaciones complejas. Dependienndo de lo que se quiere llevar a cabo para crear una aplicación o servicio, se neceita de una buena conciencia de la nube y cómo funciona en ella. Para ser específicos, en cuanto a la seguridad y la privacidad y políticas de Azure.

---
## Requisitos
 - Tener una cuenta de Azure para realizar la práctica en su [Portal](https://portal.azure.com/#home) (si aún no se cuenta con alguna, se puede hacer el registro en el siguiente [enlace](https://azure.microsoft.com/es-mx/free/)).
 - Contar con una suscripción activa de Azure para poder realizar la práctica (también en el enlace anterior indica cómo obtener una suscripción).

---
## Instrucciones
1. Una vez creada la cuenta y suscripción en Azure, se deberá acceder al Portal de Azure[*](https://portal.azure.com/#home).
    - Se deberá ver una interfaz similar a la siguiente:
    ![portal](https://github.com/JohnNadja/Practica-Creacion-Pagina-WordPress/blob/main/images/portal.png)
    - En la parte superior de la pantalla, se deberá ver una  caja de texto que permite escribir cómo búsqueda lo que requerimos. Para esta ocasión, la búsqueda será ***Marketplace***. O bien, se puede acceder desde [aquí](https://portal.azure.com/#view/Microsoft_Azure_Marketplace/MarketplaceOffersBlade/selectedMenuItemId/home).
    ![portal-marketplace](https://github.com/JohnNadja/Practica-Creacion-Pagina-WordPress/blob/main/images/portal-marketplace.gif)
2. Una vez dentro, podremos ver una lista de los servicios que se encuentran disponibles en el Marketplace. Para mayor facilidad de la práctica, se buscará (en la caja de texto) un servicio que se llame ***WordPress***.
![marketplace-wordpress](https://github.com/JohnNadja/Practica-Creacion-Pagina-WordPress/blob/main/images/marketplace-wordpress.gif)
    - Como se muestra, se debe seleccionar el servicio que contiene *"App Service"* dentro de su recuadro. Si se quiere obtener más información y una práctica de **App Service**, se puede consultar en el [*repositorio*](https://github.com/JohnNadja/Practica-Azure-Functions).

    - En **Plan**, únicamente seleccionamos la opción *WordPress* y pulsamos el botón de **Crear**. Nos mostrará una pantalla similar a la siguiente:
    ![wordpress-create](https://github.com/JohnNadja/Practica-Creacion-Pagina-WordPress/blob/main/images/wordpress-create.gif)

    - En su panel de Datos básicos, se deben indicar los siguientes parámetros:
    
        | Parametro | Descripción |
        | --------- | ----------- |
        |Grupo de recursos|Seleccionar el grupo de recursos al que se le asingnará a nuestro servicio. Si no existe, se puede crear uno. Ejemplo: PracticaWeb|
        |Nombre|Introducir el nombre de la página nueva|
        |Región|Seleccionar la región más cercana que esté disponible para mejor conectividad y menores tiempos de carga a la página web|
        |Sistema Operativo|Para esta ocasión, se usará ***Windows***|
        
        ![wordpress-create-success](https://github.com/JohnNadja/Practica-Creacion-Pagina-WordPress/blob/main/images/wordpress-create-success.gif)
    
    - Una vez terminado, pulsamos el botón de **Revisar y crear**. Esperamos a que se cree la nueva instancia.

3. Cuando ya esté creada la instancia, se debe acceder a ella ya sea ingresando desde la misma ventana (que se actualiza al terminar la creación) o desde el panel de inicio de Azure buscando el recurso.
    ![buscando-recurso](https://github.com/JohnNadja/Practica-Creacion-Pagina-WordPress/blob/main/images/buscando-recurso.gif)
    
4. Dentro de este recurso:
    - Hay un apartado que deice ***URL***, que es la URL de la página web que acabamos de crear.
    - Accedemos a ésta y observamos un panel de Información para rellenar los siguientes datos:
        | Parametro | Descripción |
        | --------- | ----------- |
        |Título del sitio| Introducir el título de la página|
        |Nombre de usuario| Introducir el nombre de usuario que se usará para acceder a la página|
        |Contraseña| Introducir la contraseña que se usará para acceder a la página|
        |Correo electrónico| Introducir el correo electrónico con el que se gestionará la ágina web|
        |Visibilidad en los motores de búsqueda| Marcar la casilla ya que, por esta ocasión, la página es para fines de prueba|
        
        ![wordpress-install](https://github.com/JohnNadja/Practica-Creacion-Pagina-WordPress/blob/main/images/wordpress-install.gif)
    
    - Pulsamos el botón de **Instalar WordPress** y deberá aparecer una ventana similar a la siguiente:
    ![web-success](https://github.com/JohnNadja/Practica-Creacion-Pagina-WordPress/blob/main/images/web-success.png)

4. Una vez instalado, se debe acceder a la página web con la URL. Ejemplo: https://mipracticaweb.azurewebsites.net/
![web-page](https://github.com/JohnNadja/Practica-Creacion-Pagina-WordPress/blob/main/images/web-page.png)

[***EXTRA***]
Si se quiere entrar al sitio para poder editarla, se coloca en el navegador la siguiente adición de dirección:`/wp-admin/`
![web-page-admin](https://github.com/JohnNadja/Practica-Creacion-Pagina-WordPress/blob/main/images/web-page-admin.gif)

### Listo, ya está creado un servicio de Marketplace para una página web de WordPress.

----
# **⚠Importante⚠**: 
### Recordar eliminar el grupo de recursos que se creó en Azure para evitar costos extras no deseados en caso de no ocupar el servicio.
Se puede hacer desde el panel de Azure en inicio y buscando el tipo de recurso que se llama **Grupo de Recursos**.


## Hasta aquí la finalización de la práctica.