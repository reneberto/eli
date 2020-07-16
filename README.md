
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

![alt text](https://github.com/reneberto/eli/blob/master/Flujoapp.jpeg)

* Aplicación con control de credenciales , contempla administración de usuarios.
* Aplicación permite listar, almacenar y modificar datos de cada uno de los Api rest definidos en Diagrama de Arquitectura Propuesta(aplicacion,predio,cuartel,producto,maquinaria,usuarios_tecnicos)
* Aplicación realiza la descarga de documentos , la creación , así como la generación de reportes en base a busquedas a definir.
* Aplicación con manejo de concurrencia , dada las caracteristicas del hardware se estima una capacidad de 20 usuarios concurrentes en ejecución.

## Tiempos de Proyecto (Sprint de 9 días)

![alt text](https://github.com/reneberto/Aplicacion/blob/master/DiagramaProyecto.jpeg)

## Mockup Aplicación

* Login

![alt text](https://github.com/reneberto/eli/blob/master/login.jpeg)

* Búsqueda y asignación Aplicación

![alt text](https://github.com/reneberto/eli/blob/master/busquedapredio.jpeg)


* Menu Principal Mantenedores (CRUD)

![alt text](https://github.com/reneberto/eli/blob/master/menu.jpeg)



## Consideraciones

* Código fuente es propiedad de Cliente
* Cambios de alcance afectos a cambios en presupuesto
* Capacitación de uso , instalación y cambios no consideradas en los tiempos de proyecto (Sprint) , pero se incluyen en el Proceso.
* Se utilizarán herramientas como "Trello" para la comunicación , creación de tareas y responsabilidades. 


## Glosario


```
* Api rest : Servicio que permite la creacion , actualización , eliminiación y consulta de una entidad (cliente, predio , producto etc)(CRUD)
* Aplicación (proceso de aplicar un producto a un predio)
* Sprint : Tiempo dedicado a tareas especificadas (Considera entrega)
```


