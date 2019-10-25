# Tecolotes-Inscripciones
Tarea 3

## 1. Introducción
### 1.1 Purpose

Sistema de Inscripciones para los alumnos del ITAM que permita agilizar y simplificar el proceso.


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
Las princiapales funciones que el sistema de inscripciones tiene que realizar es dar de alta y de baja materias. 

- Dar de alta: el alumno buscará dentro del repertorio de materias que se impartaran en el semestre las que el desee inscribir las seleccionará, eligirá grupos y entrarán a su horario si el sistema válida su inscripcioón. 

- Dar de baja: el alumno podrá dar de baja uno o más de sus materias inscritas.. 


### 2.3 User cases and characteristics


### 2.4 Operating Environment 
El sistema tiene que poder operar en los diferentes navegadores de forma correcta. Además, debe se debe poner ajustarse a las diferentes pantallas, ya que los usuarios pueden usar el sistema desde sus celulares o sus tabletas. 

### 2.5 Design and Implementation Constraints  
El sisitema se usará sobre todo al inicio del semestre, por lo que, es necesario considerar la cantidad de personas que van a estar usandolo al mismo tiempo. Los usarios tienen un límite de tiempo en el que pueden entrar al sistema y dar de alta su materia ciertos días en el semestre. Esto hace necesario una validación para verificar que el usuario si pude hacer la modificaciones que quiere. Asimismo, las bajas de materia solo se puden hacer dentro de un periodo del semestre. 

### 2.6 User Documentation  

### 2.7 Assumptions and Dependencies  


## 3. External Interface Requirements

### 3.1 User Interfaces
Interfaz de login: Esta interfaz contiene un recuadro en el centro de la página que presenta los siguientes elementos: un cuadro de texto para que el usuario coloque su clave única, este estará relacionado a una línea de texto que dice "Clave Única". Posteriormente, se encontrará otra línea de texto que dice "NIP" y otro cuadro de texto para que el usuario escriba su NIP. Finalmente, un botón que contiene el mensaje "Ingresar", este botón debe seleccionarse cuando se haya escrito la clave única y el NIP.

El botón de "Ingresar" realiza las siguientes validaciones:
.Si los campos están completos y correctos, direcciona a otra ventana.
.Si los campos están completos e incorrectos, arroja un mensaje especificando qué campo(s) es(son) incorrecto(s).
.Si los campos están incompletos, arroja un mensaje indicando que los campos deben ser llenados.

### 3.2 Hardware Interfaces

### 3.3 Software Interfaces

### 3.4 Communication Interfaces

