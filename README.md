## <p align="center">PRACTICA Nº1</p>

## <p align="center">SISTEMAS EMPRESARIALES</p>

|||
|----------|-------------|
|Carrera:| Ingenieria De Sistemas|
|Materia:| Tecnologias Emergentes II|
|Apellidos y Nombres:| Calla Mendoza Miguel Angel|
|C.I.:| 9931774 L.P.|
|Lugar y Fecha:| El Alto - 2019|

### 1. Explique que son los sistemas empresariales

El sistema de información empresarial constituye el conjunto de recursos de la empresa que sirven como soporte para el proceso básico de captación, transformación y comunicación de la información.
Un sistema de información debe ser eficaz y eficiente. Es eficaz si facilita la información necesaria, y es eficiente si lo realiza con los menores recursos posibles.

Un SIE debe adaptarse a las necesidades concretas de cada organización y a su estructura organizativa. Cuando se piensa en una implantación nunca se parte de cero pues todas las empresas disponen de algún tipo de información, más o menos rudimentario, con distintos grados de calidad/fiabilidad y con niveles de accesibilidad mayores o menores, etc. Esa información debe contemplarse como parte del SIE.

### 2. Describa cuales son las características más importantes de una aplicación empresarial

- Acceso a bases de datos

- Operaciones transaccionales

- Escalables: Horizontal y vertical

- Disponibles: prestan servicios

- Seguras

- Permiten integración

- Arquitectura multicapa

### 4.	Explique cuáles son las diferencias entre la escalabilidad horizontal y escalabilidad vertical

Escalabilidad horizontal puede aumentar componentes. 

Escalabilidad vertical moderniza o actualiza los componentes que existen.


### 5.	Que es un servidor Web y que es un servidor de aplicaciones

- Un Servidor Web es una computadora que provee servicios a otras computadoras.

- Un Servidor de Aplicaciones es un dispositivo de software que proporciona servicios de aplicación a otras computadoras.


### 6.	Con un gráfico explique cómo funciona un protocolo HTTP

![protocolo HTTP](http://2.bp.blogspot.com/_jUCZth_DkjU/TID-jK9rWcI/AAAAAAAAAAQ/3JNIssF_KeQ/s1600/protocolo.png)


### 7. Explique los elementos importantes de REQUEST en HTTP

![HTTP_Request](https://mdn.mozillademos.org/files/13687/HTTP_Request.png)

- Un método HTTP,  normalmente pueden ser un verbo, como: GET, POST o un nombre como: OPTIONS o HEAD, que defina la operación que el cliente quiera realizar. El objetivo de un cliente, suele ser una petición de recursos, usando GET, o presentar un valor de un formulario HTML, usando POST, aunque en otras ocasiones puede hacer otros tipos de peticiones. 

- La dirección del recurso pedido; la URL del recurso, sin los elementos obvios por el contexto, como pueden ser: sin el  protocolo (http://),  el dominio (aquí developer.mozilla.org), o el puerto TCP (aquí el 80). 

- La versión del protocolo HTTP.

- Cabeceras HTTP opcionales, que pueden aportar información adicional a los servidores.

- O un cuerpo de mensaje, en algún método, como puede ser POST, en el cual envía la información para el servidor.


### 8. Explique los elementos importantes de RESPONSE en HTTP

![HTTP_Response](https://mdn.mozillademos.org/files/13691/HTTP_Response.png)

- La versión del protocolo HTTP que están usando.

- Un código de estado, indicando si la petición ha sido exitosa, o no, y debido a que.

- Un mensaje de estado, una breve descripción del código de estado. 

- Cabeceras HTTP, como las de las peticiones.

- Opcionalmente, el recurso que se ha pedido.


### 9. Describa con un gráfico la arquitectura Java EE

![Java EE](https://users.dcc.uchile.cl/~jbarrios/J2EE/arq.gif)

- En la Capa Cliente: se ubican los clientes de nuestra aplicación y tienen diversas naturalezas.

- La Capa de Presentación: contiene toda la lógica de interacción entre el programa y el cliente y viceversa. Además, es la encargada de controlar las acciones entre el usuario y la lógica del negocio.

- La Capa de Lógica de Negocio: tiene a su cargo el núcleo de la aplicación. Debe ser mantenible, reutilizable, extensible y flexible.

- La Capa de Integración: se llevan a cabo tareas de integración con otros sistemas.

- En la Capa de Recursos: se localizan los sistemas de almacenamien to disponibles, como bancos de ficheros y bases de dato.


### 11. Investigue los métodos más utilizados de las clases HttpServlet, HttpServletRequest y HttpServletResponse, y para cada uno de los métodos muestre un ejemplo

**HttpServletRequest**

- El método getParameter devuelve el valor de un parámetro nombrado. Si nuestro parámetro pudiera tener más de un valor, deberíamos utilizar getParameterValues en su lugar. El método getParameterValues devuelve un array de valores del parámetro nombrado.

- El método getParameterNames proporciona los nombres de los parámetros.

- Para peticiones GET de HTTP, el método getQueryString devuelve en un String una línea de datos desde el cliente. Debemos analizar estos datos nosotros mismos para obtener los parámetros y los valores.

- Para peticones POST, PUT, y DELETE de HTTP.

Si esperamos los datos en formato texto, el método getReader devuelve un BufferedReader utilizado para leer la línea de datos.    
Si esperamos datos binarios, el método getInputStream devuelve un ServletInputStream utilizado para leer la línea de datos.

**HttpServletResponse**

- El método getWriter devuelve un Writer

- El método getOutputStream devuelve un ServletOutputStream

Se utiliza el método getWriter para devolver datos en formato texto al usuario y el método getOutputStream para devolver datos binarios.    

Si cerramos el Writer o el ServletOutputStream después de haber enviado la respuesta, permitimos al servidor saber cuando la respuesta se ha completado.
