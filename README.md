# Práctica 2 - Esquemas XML (XSD)

Esta práctica contiene ejercicios para aprender a definir esquemas XML utilizando XML Schema Definition (XSD). Los ejercicios van desde esquemas simples hasta restricciones avanzadas y tipos complejos.

## Estructura de la Práctica

### EJERCICIO 7: Esquema Simple 1
- **Archivos**: `simple1.xml`, `simple1.xsd`
- **Descripción**: Crear un documento XML `simple1.xml` con datos personales de un alumno y un esquema `simple1.xsd` para validarlo. Incluye elementos como nombre, dni, dirección, edad y teléfono.

### EJERCICIO 8: Esquema Simple 2
- **Archivos**: `simple2.xml`, `simple2.xsd`
- **Descripción**: Crear el esquema `simple2.xsd` para validar el documento XML `simple2.xml`, que describe un libro con título, autor, fecha, ISBN y editorial.

### EJERCICIO 9: Restricciones 1
- **Archivos**: `restriccion1.xml`, `restriccion1.xsd`
- **Descripción**: Modificar `simple1.xml` cambiando la edad a 20 y guardarlo como `restriccion1.xml`. Crear `restriccion1.xsd` basado en `simple1.xsd`, añadiendo restricción numérica para la edad (entre 16 y 25 años).

### EJERCICIO 10: Restricciones 2
- **Archivos**: `restriccion2.xml`, `restriccion2.xsd`
- **Descripción**: Añadir el elemento `<sexo>` con valor "M" a `restriccion1.xml` y guardarlo como `restriccion2.xml`. Modificar `restriccion1.xsd` para crear `restriccion2.xsd`, permitiendo solo "M" o "H" en sexo mediante enumeración y definiendo un tipo personalizado `tipoSexo`.

### EJERCICIO 11: Restricciones 3
- **Archivos**: `restriccion3.xsd`
- **Descripción**: Crear `restriccion3.xsd` basado en `restriccion2.xsd`, añadiendo restricciones de patrón con expresiones regulares: DNI debe tener 8 dígitos seguidos de una letra mayúscula, teléfono solo números.

### EJERCICIO 12: Restricciones 4
- **Archivos**: `restriccion4.xsd`
- **Descripción**: Modificar `restriccion3.xsd` para añadir restricciones de longitud: DNI exactamente 9 caracteres (8 dígitos + 1 letra), teléfono entre 9 y 12 dígitos. Guardar como `restriccion4.xsd`.

### EJERCICIO 13: Tipos Complejos
- **Archivos**: `complejo.xml`, `complejo.xsd`
- **Descripción**: Crear `complejo.xsd` para validar `complejo.xml`, que incluye un elemento `alumno` con DNI como atributo y `direccion` como tipo complejo anidado con calle, numero, ciudad, cp y provincia.

## Objetivos de Aprendizaje
- Comprender la sintaxis básica de XSD.
- Aprender a definir tipos simples y complejos.
- Aplicar restricciones y validaciones a los datos XML.
- Usar enumeraciones y patrones para validar formatos específicos.
- Crear estructuras anidadas con tipos complejos.

## Validación
Para validar un archivo XML contra su esquema XSD, puedes usar herramientas como:
- Validadores online de XML/XSD.
- Librerías en lenguajes de programación (ej. Java, Python).
- Editores de XML que soporten validación automática.
