# FiUber-Taller-2-7552--FIUBA

## Objetivo
El objetivo del proyecto es crear una aplicación móvil de transporte que cuente con las principales funcionalidades similar a Uber, destinada tanto a choferes como pasajeros.
A su vez, también se busca crear un sitio web que funcione como back-office destinado a los administradores del sistema.

### Enunciado
El enunciado completo junto con toda la información detallada, incluyendo:
* Descripción
* Requisitos Funcionales
  * Épicas 
  * Historias de usuario
* Requisitos No Funcionales

Se puede consultar en el siguiente enlace: [Enunciado proyecto FiUber](https://taller-de-programacion-2.github.io/tasks/statement/2022/2/enunciado/)


## DEMO
### Aplicación móvil
https://github.com/imontecalvo/FiUber-Taller-2-7552--FIUBA/assets/82344492/7a327d50-a73f-42a5-94ba-6854de346cde

### Backoffice web
https://github.com/imontecalvo/FiUber-Taller-2-7552--FIUBA/assets/82344492/10ab00c2-e8a0-4e61-93e3-dac5c74002f3

## Documentacion
La documentación del backend y los manuales de usuario, tanto de la aplicación móvil como del backoffice, se encuentran en el siguiente enlace: [Documentacion del proyecto](https://fiubergrupo6.github.io/fiuber-documentacion)

## Arquitectura
Se utilizó una arquitectura de microservicios, donde cada uno de los cuatro microservicios (Cuentas, Viajes, Pagos y Métricas) se mantiene aislado, desplegado de forma independiente, brinda una determinada API y posee su propia base de datos.

Por otro lado, se encuentra un gateway que hace de intermediario entre el frontend y los microservicios evitando una comunicación directa con los mismos y encargándose de la creación o validación del token cuando corresponda.

A continuación, se puede ver un diagrama que ilustra esta arquitectura, junto con las interacciones que ocurren entre los microservicios en cuestión, las cuales suceden de forma interna y directa sin pasar por el gateway.

<p align="center">
  <img src="https://github.com/imontecalvo/FiUber-Taller-2-7552--FIUBA/assets/82344492/90b5841b-380f-463c-b11e-7e73a050cfa4" />
</p>

## Microservicios
* **Cuentas**: Se encarga de todas las funciones relacionadas a la creación, modificación, eliminación y obtención de cuentas, ya sean usuarios (choferes y pasajeros) como administradores del backoffice.
  
* **Viajes**: Se encarga de todas las funciones relacionadas a la realización de un viaje incluyendo el inicio de un viaje, la búsqueda de pasajero por parte del chofer, confirmación de viaje y la finalización del mismo.
  
* **Métricas**: Se encarga de todas las funciones relacionadas a la creación, modificación y obtención de métricas relacionadas a los viajes, usuarios y transacciones.
  
* **Pagos**: Se encarga de todas las funciones relacionadas a la creación y obtención de wallets, realización de depósitos y retiros, y obtención de información de transacciones realizadas.


Los endpoints de cada una de las APIs que proporcionan estos microservicios se encuentran en la documentación: [Endpoints de microservicios](https://fiubergrupo6.github.io/fiuber-documentacion/pages/backend-doc.html)

## Stack utilizado
### Backend
* Node.js + Express
* Python + Flask
  
### Frontend
* React (backoffice web)
* React Native (aplicación móvil)
  
### Base de datos
* PostgreSQL
* MongoDB

## Integrantes
* [Federico Mangiaterra](https://github.com/fedemangiaterra)
* [Franco Ferrer Vieyra](https://github.com/francoferrerv)
* [Franco Nicolini](https://github.com/franconicolini1)
* [Gonzalo Rizzo Ehreböck](https://github.com/grizzoeh)
* [Ignacio Montecalvo](https://github.com/imontecalvo)
