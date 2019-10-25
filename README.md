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
-Si los campos están completos y correctos, direcciona a otra ventana.
-Si los campos están completos e incorrectos, arroja un mensaje especificando qué campo(s) es(son) incorrecto(s).
-Si los campos están incompletos, arroja un mensaje indicando que los campos deben ser llenados.

Interfaz de inscripción general: Esta interfaz envía a una ventana con cuatro pestañas distintas. Las pestañas tienen los siguientes nombres: "Inscripción", "Bajas", "Listas de espera" y "Vista previa del horario".
La pestaña de "Inscripción" se muestra automáticamente al momento de entrar a esta interfaz, en ella se muestra un campo con una lista desplegable que contiene el nombre de todas las materias disponibles, al seleccionar una materia, de manera automática se muestran todos los grupos en los que se impartirá esa materia. En cada fila hay, por orden, un checkbox, una letra que indica el estatus del grupo ('A' si es abierto, 'LE' si es para lista de espera) la clave de la materia, el nombre del profesor que la impartirá, los días en los que se impartirá, el horario en el que se impartirá y la clave del grupo; al final del despliegue de grupos disponibles, aparece un botón centrado que dice "Registrar", este debe seleccionarse cuando se haya elegido un grupo con el checkbox.

El botón de "Registrar" realiza las siguientes validaciones:
.Si el registro está disponible en el grupo, muestra un mensaje que indica que el grupo fue registrado correctamente e indica si es en lista de espera en caso de que lo sea.
.Si al momento de 

### 3.2 Hardware Interfaces

### 3.3 Software Interfaces

### 3.4 Communication Interfaces

## 4. System Features

### 4.1 [Entrada al sistema con credenciales de usuario](https://github.com/ITAM-IngenieriaSoftware-2019/Tecolotes-Inscripciones/issues/1)
### 4.2 [Inscribir materia](https://github.com/ITAM-IngenieriaSoftware-2019/Tecolotes-Inscripciones/issues/2)
### 4.3 [Dar de baja materia](https://github.com/ITAM-IngenieriaSoftware-2019/Tecolotes-Inscripciones/issues/3)

## 5. Other Nonfunctional Requirements

### 5.1 Performance Requirements
Es necesario considerar que el sistema debe soportar ser utilizado por muchos alumnos al mismo tiempo. Desde el inicio de sesión hasta la alta y baja de materias, el sistema debe aguantar una carga de por lo menos 500 alumnos. Considerando que cada alumno busca 8 e inscribe o da de baja 6 materias en promedio durante su sesión, se requiere que la base de datos pueda soportar aproximadamente 5000 lecturas y 3500 modificaciones por hora. Además, los tiempos de respuesta para las solicitudes de lectura no deben de rebasar 0.1 segundos, y las demás solicitudes deben completarse por debajo del segundo.


### 5.2 Safety Requirements
Al inicio del semestre, en caso de ocurrir una falla generalizada a cierto porcentaje de los usuarios, es necesario desactivar el sistema y recorrer los horarios de entrada al sistema de los alumnos hasta que la falla quede corregida para evitar que alumnos pierdan grupos o materias debido a que éstos se llenen con alumnos de horarios posteriores.
En caso de daños a la base de datos, es necesario llevar un registro de las transacciones llevadas a cabo por los alumnos así como tener un método de recuperación que permita restablecer una versión anterior de la base y que aplique las transacciones del registro.

### 5.3 Security Requirements
Es necesario contar con un método de encripicón para mantener seguras las contraseñas de los usuarios al momento de que inicien sesión en el sistema. Asimismo, la recuperación de contraseña debe asociarse al correo escolar del usuario y también contar con métodos de encripción. Por último, se debe establecer un período de inactividad de 5 minutos tras el cual la sesión del usuario debe expirar y debe ser sacado del sistema de forma automática.

### 5.4 Software Quality Attributes
- **Portabilidad**. El sistema debe de funcionar en los navegadores más comunes:
	- Google Chrome
	- Safari
	- Microsoft Edge
	- Internet Explorer
	- Mozilla Firefox
- **Confiabilidad**. El sistema debe realizar las transacciones correctamente y tener la disponibilidad requerida para asegurar una confiabilidad del 98% en cada sesión.
- **Mantenibilidad**.
- **Facilidad de testeo**.
- **Reusabilidad**.

### 5.5 Business Rules
El sistema puede ser ingresado por los alumnos del ITAM en todo momento. Sin embargo, las funciones de alta y baja de materias solamente están disponibles en fechas y horarios asignados por el instituto. Fuera de este tiempo, los alumnos solamente pueden ingresar al sistema para ver su información.
