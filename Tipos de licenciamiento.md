# **TIPOS DE LICENCIAMIENTO**
## *MIT*
Licencia que suele ser utilizada cuando el creador del software quiere que el código sea accesible para el mayor número de desarrolladores
y trabajos derivados posible y no le importa dónde o cómo vaya a ser el futuro uso del código, ya que éste puede reescribirse bajo una licencia 
del tipo que sea, incluso privativa.

## *GNU*
Licencia de derecho de autor ampliamente usada en el mundo del software libre y código abierto que garantiza a los usuarios o compañías la libertad 
de usar, estudiar, compartir (copiar) y modificar el software.

## *Apache*
Licencia de software libre permisiva creada por la Apache Software Foundation (ASF). Esta licencia requiere la conservación del aviso de derecho de autor
y el descargo de responsabilidad, pero no es una licencia copyleft, ya que no requiere la redistribución del código fuente cuando se distribuyen versiones
modificadas. 

La diferencia entre estos tres tipos de licenciamiento es que MIT (Massachusetts Institute of Technology) es más accesible pero a la vez mo tiene tanto como el avi
el aviso del derecho de auto como la licencia Apache o GNU(General Public License).

#  PATRON DE DISEÑO *MVC (MODEL VIEW CONTROLLER)* Y *DDD(DOMAIN DRIVEN DESIGN)*

## **MVC**
El MVC o Modelo-Vista-Controlador es un patrón de arquitectura de software que, utilizando 3 componentes *(Vistas, Models y Controladores)* separa la lógica de la aplicación de la lógica de la vista en una aplicación. Es una arquitectura importante puesto que se utiliza tanto en componentes gráficos básicos hasta sistemas empresariales; la mayoría de los frameworks modernos utilizan MVC.

1. El **Modelo** que contiene una representación de los datos que maneja el sistema, su lógica de negocio, y sus mecanismos de persistencia.
2. La **Vista**, o interfaz de usuario, que compone la información que se envía al cliente y los mecanismos interacción con éste
3. El **Controlador**, que actúa como intermediario entre el Modelo y la Vista, gestionando el flujo de información entre ellos y las transformaciones para adaptar los datos a las necesidades de cada uno.

### El modelo es el responsable de:
- *Acceder a la capa de almacenamiento de datos.*
- *Define las reglas de negocio (la funcionalidad del sistema).*
- *Lleva un registro de las vistas y controladores del sistema.*
- *Si se está ante un modelo activo, notificará a las vistas los cambios*
 *que en los datos pueda producir un agente externo.*

## La vista es responsable de:

- *Recibir datos del modelo y los muestra al usuario.* 
- *Pueden dar el servicio de "Actualización()", para que sea invocado por el controlador o por el modelo.*

## El constrolador es responsable de:

- *Recibir los eventos de entrada *
- *Contiene reglas de gestión de eventos, del tipo "SI Evento Z, entonces Acción W". Estas acciones pueden* 
*suponer peticiones al modelo o a las vistas.*

![Model View Controller](https://si.ua.es/es/documentacion/asp-net-mvc-3/imagenes/introduccion/flujo-mvc.png)



## **DDD**

Representa distintas claves, terminología y patrones utilizados para desarrollar software donde el dominio 
es lo más central e importante de una determinada organización.

Sus principios se basan en:

- Colocar los modelos y reglas de negocio de la organización, en el core de la aplicación
- Basar nuestro dominio complejo, en un modelo de software.
- Se utiliza para tener una mejor perspectiva a nivel de colaboración entre expertos del dominio 
y los desarrolladores, para concebir un software con los objetivos bien claros.

![Domain Driven Design](https://cdn-images-1.medium.com/max/1600/1*S0vOjV9QgK7bsJeJhASyYQ.png)


