# Tecolotes-Inscripciones
Tarea 3

## 1. Introducción
### 1.1 Purpose

Sistema de Inscripciones para los alumnos del ITAM que permita agilizar y simplificar el proceso. El sistema esta pensado como un subsistema de los servicios en linea de la universidad y se ayudara de estos para su funcionamiento. 


### 1.2 Document conventions 

El documento se basa en la jerarquia especificada por la IEEE. Par la estimacion de la complejidad de los diferentes componentes utilizamos una escla de elote, donde de menor a mayor tenemos:

    1. Esquite
    2. Elote asado
    3. Elote con mayonesa, queso y chile del que no pica
    4. Elote con mayonesa, queso y chile del que pica


### 1.3 Intended Audience and Reading Suggestions

El documento está planeado para ser leído por desarrolladores, por lo que el resto del documento contendrá los detalles técnicos necesarios para el desarrollo del proyecto. Recomendamos que se siga el orden lógico dado para su lectura. 


### 1.4 Product Scope 

El objetivo de este proyecto es proveer un sistema de inscripciones para los alumnos del ITAM que permita agilizar y facilitar el proceso de inscripciones al inicio de cada semestre, comsiderando alta de materias, baja de materias, prerrequisitos, carga académica, listas de espera, entre otras cosas.

### 1.5 References

Por el momento no se cuenta con ninguna referencia externa

## 2. Overall Description

### 2.1 Product Perspective
El sistema de inscripciones sustituira el actual sistema de inscripciones debido a su ineficiencia. Se busca mejor la experiencia del usuario al entrar al sistema de inscripciones y optimizar la construcción del sistema. 

### 2.2 Product Function
Las principales funciones que el sistema de inscripciones tiene que realizar es dar de alta y de baja materias. 

- Dar de alta: el alumno buscará dentro del repertorio de materias que se impartaran en el semestre las que el desee inscribir las seleccionará, eligirá grupos y entrarán a su horario si el sistema válida su inscripcioón. 

- Dar de baja: el alumno podrá dar de baja uno o más de sus materias inscritas.

### 2.3 User cases and characteristics
Los usaurios que usarán el sistema son los alumnos, profesores y directores de carrera. Los alumnos podrán inscribir o dar de baja materia. Los profesores y directores de carrera podrán ver las materias, los alumnos inscritos a cada materia y aceptar o rechazar las listas de espera. 

### 2.4 Operating Environment 
El sistema tiene que poder operar en los diferentes navegadores de forma correcta. Además, debe se debe poner ajustarse a las diferentes pantallas, ya que los usuarios pueden usar el sistema desde sus celulares o sus tabletas. 

### 2.5 Design and Implementation Constraints  
El sisitema se usará sobre todo al inicio del semestre, por lo que, es necesario considerar la cantidad de personas que van a estar usandolo al mismo tiempo. Los usarios tienen un límite de tiempo en el que pueden entrar al sistema y dar de alta su materia ciertos días en el semestre. Esto hace necesario una validación para verificar que el usuario si pude hacer la modificaciones que quiere. Asimismo, las bajas de materia solo se puden hacer dentro de un periodo del semestre. 

### 2.6 User Documentation  
Por el momento no hay documentación externa de la que nos hemos apoyado. Sin embargo, consideramos que en un futuro podriamos usar bootstrap para ayudarnos a realizar el sistema. 

### 2.7 Assumptions and Dependencies  
Se usará la base de datos de ITAM, la cual autalmente ya se usa para el sistema de inscripciones. Además, de los servicios que consideremos necesarios para desarrollar nuestro sistema. 
