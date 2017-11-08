# HTTP

---

### Características
#### de HTTP

![Press Down Key](assets/down-arrow.png)

+++
###### Protocolo de **Capa de Aplicación** utilizado para enviar documentos hipermedia (HTML).
###### Sigue el modelo cliente-servidor, en el que un **cliente** establece la conexión, realiza una **petición**
###### a un servidor y espera su respuesta. Es un protocolo sin estado, por lo que **no guarda ningún dato**.
###### Aunque suele tratarse de una conexión de tipo **TCP/IP** puede ser usado sobre la capa de transporte.
###### HTTP es **sencillo** (está pensado para ser leido e interpretado de forma fácil) y **extensible**
---

### Típica
#### Sesión

![Press Down Key](assets/down-arrow.png)

+++
###### Una sesión consta de **tres fases**:
###### El cliente establece una conexión TCP.
###### El cliente manda su petición y espera por la respuesta.
###### El servidor procesa la petición y responde con un código de estado y los datos correspondientes.
###### Iniciar una conexión en HTTP, por lo que deberemos iniciar una conexión en el *protocolo correspondiente a la capa de comunicación subyacente*, que normalmente es **TCP**
###### Una vez la conexión está establecida el cliente puede mandar una *petición de datos*, la cual consta de **tres fases**:
###### Añade una línea con la dirección del documento pedido y la versión del protocolo HTTP.
###### Bloque que representa las cabeceras de la petición.
###### Bloque de datos opcional, que contiene datos usados por el método POST.
---

#### **Cabeceras** HTTP

![Press Down Key](assets/down-arrow.png)

+++
###### Las cabeceras HTTP permiten que el cliente y el servidor pasen información adicional con la petición o la respuesta.
###### La **cabecera de la petición** es de la forma **nombre**:**valor**.
###### Las cabeceras pueden agruparse de acuerdo a su contexto:
###### **Generales**: Cabeceras que se aplican tanto a la petición como a la respuesta.
###### **De petición**: Contiene información sobre la búsqueda.
###### **De respuesta**: información adicional sobre la respuesta.
---

#### **Peticiones** HTTP

![Press Down Key](assets/down-arrow.png)

+++
###### HTTP define un conjunto de métodos de petición para indicar la acción que se desea realizar para un recurso determinado.
###### **Método GET**
###### Solicita una representación de un recurso específico. Las peticiones que usan el método GET sólo deben recuperar datos.
###### **Método POST**
###### El método POST se utiliza para enviar una entidad a un recurso en específico, causando a menudo un cambio en el estado o efectos secundarios en el servidor.
---

#### **Respuestas** HTTP

![Press Down Key](assets/down-arrow.png)

+++
###### Después de recibir e interpretar un mensaje de solicitud, el servidor responde con un mensaje de respuesta HTTP
###### El **elemento de estado** es un número de 3 dígitos, donde el **primer dígito** define la *clase de respuesta* y los **dos últimos** dígitos *no tienen ningún papel*.
###### 1XX: Esto significa que la solicitud fue recibida y el proceso continúa.
###### 2XX: Esto significa que la acción se ha recibido correctamente, comprendido y aceptado.
###### 3XX: Significa además hay que tomar medidas con el fin de completar la solicitud.
###### 4XX: Esto significa que la solicitud contiene sintaxis incorrecta o no se puede cumplir.
###### 5XX: Esto significa que el servidor incumplido una petición aparentemente válida.
---

#### Cookies

![Press Down Key](assets/down-arrow.png)

+++
###### Una cookie de navegador es una pequeña pieza de datos que un servidor envía al navegador del usuario.
###### Las cookies se usan generalmente para decirle al servidor que dos peticiones tiene su origen en el mismo navegador web,
###### lo que permite, por ejemplo, mantener la sesión de un usuario abierta.
###### Las cookies se utilizan principalmente por tres motivos:
###### **Gestión de Sesión**
###### **Personalización**
###### **Rastreo**
---

#### Evolución de HTTP

![Press Down Key](assets/down-arrow.png)

+++
###### Fue inventado por Tim Berners-Lee entre los años 1989-1991.
###### HTTP ha evolucionado, desde un *protocolo destinado al intercambio de archivos en un entorno de un laboratorio*
###### hasta *lo que es ahora Internet*.
###### WWW se desarrolló sobre los protocolos existentes TCP e IP, basándose en cuatro bloques:
###### + Un formato de texto para representar documentos de hiper-texto (HTML).
###### + Un protocolo sencillo para el intercambio de esos documentos (HTTP).
###### + Un cliente que muestre (e incluso pueda editar) esos documentos (WWW).
###### + Un servidor para dar acceso a los documentos, una versión temprana (httpd)
###### Desde ese momento, se comenzaron a implementar mejoras, comenzando por el llamado "Método de una sola linea", basado en el método GET, hasta la aparición del HTTP/2
---

#### Características
#### HTTP 2.0

![Press Down Key](assets/down-arrow.png)

+++
###### El protocolo HTTP/2, tiene notables diferencias fundamentales respecto a la versión anterior HTTP/1
###### **1)** Es un protocolo binario, en contraposición a estar formado por cadenas de texto, tal y como estában basados sus protocolos anteriores.
###### **2)** Es un protocolo multiplexado. Peticiones paralelas pueden hacerse sobre la misma conexión.
###### **3)** Comprime las cabeceras, lo cual elimina la duplicación y retardo en los datos a transmitir.
---
