
# Propuesta desarrollo Software gestión auditoria 
Diseño aplicación gestión tratamientos y aplicación de productos sobre predios  

## Arquitectura Propuesta

![alt text](https://github.com/reneberto/eli/blob/master/elidiag.jpeg)

Se utilizará un servidor en la nube en este caso se propone un linode Caracteristicas:
 1 CPU, 50GB Storage, 2GB RAM
* Los datos serán almacenados en una base de datos mariaDb(relacional) , se creará el modelo de datos segun necesidad , estos datos son almacenados en un volumen persistente.
* El acceso a datos se realizará mediante servicios Api Rest utilizando JSON desarrollados con Java Spring boot , el consumo de estos servicios se realizará en un frontend (aplicación web) la cual se encontrará disponible desde cualquier dispositivo con acceso a Internet.
```
Toda la arquitectura sobre contenedores Docker para una escalabilidad limpia 
y fácil migración en caso de ser necesario
```

Mas información en: 
* https://www.linode.com
* https://mariadb.org/
* https://www.docker.com/
* https://spring.io/projects/spring-boot

## Diagrama Uso Aplicación (versión inicial)

![alt text](https://github.com/reneberto/eli/blob/master/flujoapp.jpeg)

* Aplicación con control de credenciales , no se contempla administración de usuarios en caso de ser necesario se puede agregar.
* Aplicación permite listar, almacenar y modificar datos de clientes existentes 
* Aplicación realiza la descarga de documentos , la creación y envío automático a través de correo electrónico

## Tiempos de Proyecto (Sprint de 8 días)

![alt text](https://github.com/reneberto/Aplicacion/blob/master/DiagramaProyecto.jpeg)

## Mockup Aplicación

* Login:

![alt text](https://github.com/reneberto/Aplicacion/blob/master/login.jpeg)
```
Ingreso Controlado por Usuario y Contraseña
```
* Menu Principal:

![alt text](https://github.com/reneberto/Aplicacion/blob/master/Principal.jpeg)
```
Selección de Clientes y Documentos
```
* Clientes:

![alt text](https://github.com/reneberto/Aplicacion/blob/master/Clientes.jpeg)
```
Creación , búsqueda y modificación de Clientes
```
* Documento:

![alt text](https://github.com/reneberto/Aplicacion/blob/master/Documentos.jpeg)
```
Creación de Documentos asociados por búsqueda de cliente , descarga del documento y envío
a través de correo electrónico
```

## Consideraciones

* Código fuente es propiedad de Megaservi
* Cambios de alcance afectos a cambios en presupuesto
* Capacitación de uso , instalación y cambios no consideradas en los tiempos de proyecto (Sprint) , pero se incluyen en el Proceso.
* Se utilizarán herramientas como "Trello" para la comunicación , creación de tareas y responsabilidades. 

