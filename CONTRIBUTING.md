## Contribuir a gestor-inventarios-it
Damos las gracias y bienvenidas sean todas las correcciones y mejoras en el desarrollo del código de gestor-inventarios-it, pruebas y documentación. 
Esta guía detalla como contribuir en el proyecto de una manera que sea eficiente para toda la comunidad.


1. [Prerequisitos](#1-prerequisitos)
2. [Preparación de ambiente local](#2-preparación-de-ambiente-local)
3. [Detección y solución de issues](#3-detección-y-solución-de-issues)
  - [Detección de issues](#31-detección-de-issues)
  - [Solución de issues](#32-solución-de-issues)
4. [Agregar nuevas características](#4-agregar-nuevas-características)
5. [Actualizar mi repositorio local](#5-actualizar-mi-repositorio-local)
6. [¿Dudas, consultas, información?](#6-dudas-consultas-información)


### 1. Prerequisitos 

1.1 [Leer el Manual de gestor-inventarios-it](/docs/gestor-inventarios-it.docx) 
En costrucción 

1.2 Tener clara la normalización de código fuente

1.3 Documentar y comentarizar correcciones y/o nuevos desarrollos.

[Volver](#contribuir-a-simple)


### 2. Preparación de ambiente local

2.1 Realizar Fork del repositorio https://github.com/wcadena/gestor-inventarios-it a tu cuenta GitHub

2.2 Clonar el proyecto forkeado desde tu cuenta GitHub. Ejemplo:
  ```console
  https://github.com/isairey/gestor-inventarios-it.git
  ```
2.3 Agregar el repositorio padre como origen remoto. Ejemplo:
  ```console
  git remote add upstream https://github.com/isairey/gestor-inventarios-it.git
  ```
2.4 Luego de clonado el proyecto, crear la rama beta para empezar a trabajar. Ejemplo:
  ```console
  git checkout -b beta
  ```
2.5 Realizar los commits con una descripción sobre la o las nuevas  funcionalidades
  ```console
  git commit -m “ Modifico funcionalidad manager”
  ```
2.6 Generar un push hacia la rama beta del proyecto forkeado. Ejemplo:
  ```console
  git push origin beta
  ```
2.7 Generar un pull request hacia la rama beta del proyecto origen por la interfaz de Github

[Volver](#contribuir-a-simple)

### 3. Detección y solución de issues

#### 3.1 Detección de issues 
Antes de ingresar la incidencia, se recomienda buscar dentro del tracker de issues entradas similares 
para verificar que la incidencia ya haya sido reportada o resuelta.

Para ingresar un issue, favor usar la siguiente plantilla en el área de descripción:

3.1.1 Resumen
(Resumir el issue en una sentencia. Cual es el error o que esperas que suceda)

3.1.2 Pasos para reproducir
(Como se reproduce el issue)

3.1.3 Comportamiento esperado
(Lo que debe ver en su lugar)

3.1.4 En lo posible, capturas de pantalla relevantes
(Capturas de pantalla que ayuden a reproducir el error)

[Volver](#contribuir-a-simple)

#### 3.2 Solución de issues
Lo principal es primero cumplir con los prerequisitos, luego :

3.2.1 Comentar el Issue y detallar la solución que se entregará.

3.2.2 Realizar los commits con una descripción sobre la o las correcciones realizadas"
```console
git commit -m "Modifico funcionalidad manager"
```
3.2.3 Generar un push hacia la rama beta del proyecto forkeado. Ejemplo:
```console
git push origin beta
```
3.2.4 Generar un pull request hacia la rama beta del proyecto origen por la interfaz de Github  

[Volver](#contribuir-a-simple)

### 4. Agregar nuevas características
Para agregar nuevas caracteristicas, es necesario primero cumplir con los prerequisitos

4.1 Abrir un ISSUE, indicando cual es la caracteristica, funcionalidad o complemento que falta en Inventarios

4.2 Comentar el Issue, agregar la solución que se entregara.

4.3 Realizar los commits con una descripción sobre la o las nuevas funcionalidades:
```console
git commit -m "Modifico funcionalidad manager"
```
4.4 Generar un push hacia la rama beta del proyecto forkeado. Ejemplo:
```console
git push origin beta
```
4.5 Generar un pull request hacia la rama beta del proyecto origen por la interfaz de Github 

[Volver](#contribuir-a-simple)

### 5. Actualizar mi repositorio local
 Si queremos actualizar nuestro repositorio con los cambios del repositorio padre Inventarios debemos seguir los siguientes pasos
```console
git fetch upstream

git merge upstream/master
```
  Donde master indica la rama del repositorio padre a actualizar

[Volver](#contribuir-a-simple)

### 6. ¿Dudas, consultas, información?
contáctese con nosotros al correo wcadena@outlook.com

[Volver](#contribuir-a-simple)


## Traducción

Las traducciones se hacen a partir del [repo original](https://github.com/isairey/gestor-inventarios-it). Los aportes de traducción pueden ser de diferentes maneras:

 1. Traducir los términos pendientes o nuevos.
 2. Corregir traducciones existentes.

Sin embargo, al traducir queremos utilizar un español internacional.

 > 💁 **Importante** Las definiciones originales (en inglés) están incluidas en el documento en forma de comentario. A medida que traduzcas una definición al español, entonces la remueves.

## Flujo de Trabajo

 1. Busca una traducción pendiente en la columna TODO: [ver traducciones pendientes](https://github.com/isairey/gestor-inventarios-it/pendientes).
 2. Asegúrate que nadie esté trabajando en él (te puedes dar cuenta viendo que no haya nadie asignado ni nadie ha comentado que está trabajando).
 3. Sigue las reglas descritas abajo y crea tu PR.

Dicho esto, nos gustaría mantener un mínimo de consistencia a través del documento.

## Guía de estilo

 1. Las definiciones deben ser escritas utilizando las palabras más sencillas.
 2. Piense en los programadores que no tienen experiencia en programación funcional.
 3. Apreciamos más lo entendible que lo preciso.
 4. No use mucha jerga en las definiciones aunque estén definidas en otras parte del sistema.
 5. Si utilizas una jerga crea un enlace a su definición en el documento.
 

## Convenciones de Código

Laravel sigue los estándares PSR-1 y PSR-4. Y además tiene algunas recomendaciones propias. Lo que en algunos entornos llaman el ‘Laravel “flavor” of PSR-2‘. Estos son los estándares extraídos de su guía de colaboración.

He comentado después de cada estándar y resaltado en negrita los cambios con respecto al estándar PSR-2.

Si usas PhpStorm, al final de este post tienes un link para descargarte un fichero .xml para configurar el ‘Estilo de código Laravel’.
La declaración del namespace DEBE estar en la misma línea que <?php

```console
  <?php namespace Curso\Http\Controllers;
```

No existe en los estándares PSR una regla acerca de esto.
La llave de apertura de las clases DEBEN ir en la misma línea que el nombre de la clase.

```console
class SQLiteConnection extends Connection {

      protected function getDefaultQueryGrammar()
      {
          return $this->withTablePrefix(new QueryGrammar);
      }

      (...)
```

En PSR-2 recomiendan que la llave vaya en la línea siguiente.
Las funciones y estructuras de control deben seguir el estilo de llaves Allman.El estilo Allman define que la llave de apertura de las estructuras de control DEBE ir en la línea siguiente. La llave de cierre DEBE estar al mismo nivel que la de apertura. Y el cuerpo de la estructura DEBE estar indentado.

```console
 (...)

  if ($previous instanceof PDOException)
  {
      $this->errorInfo = $previous->errorInfo;
  }

  (...)
```

En PSR-2 recomiendan que la llave de apertura vaya en la misma línea separada por un espacio del paréntesis de cierre de la declaración.
Indentar con tabuladores y alinear con espacios.
En PSR-2 recomiendan indentar con espacios.
Si usas PHP-Sniffer, este paquete te permite comprobar si tu código sigue los estándares de Laravel y reformatea tu código para que sea compatible con ellos: Laravel PHP_CodeSniffer
Este es otro paquete que te ayuda a formatear tu código para que siga los estándares PSR-1 y PSR-2 y GrahamCampbell está entre uno de sus colaboradores: FriendsOfPHP/PHP-CS-Fixer
Otras convenciones de código recomendadas.

Estas convenciones no están ‘oficialmente’ recogidas en estándares. Pero te facilitarán mucho la vida como programador de PHP y te ayudarán a evitar algunos errores. Complementan y amplían las convenciones explicadas hasta ahora.

Están basadas en ‘estándares de facto’, en las recomendaciones de Symfony y en el código del Framework de Laravel.

Usa siempre el tag de apertura largo de PHP <?php. No uses el tag corto <?.
No dejes espacios antes del tag de apertura.
Entre otros motivos, el tag corto es incompatible con las especificaciones de XML.

No uses el tag de cierre de PHP ?> al final de los ficheros.Es opcional. Y cuando lo usas, si dejas espacios o líneas en blanco después de él, esos espacios pueden ir a la salida resultante del script y generar errores.Créeme, a mí me ha pasado alguna vez y es un auténtico incordio tener que revisar decenas de ficheros .php buscando espacios en blanco después del tag de cierre.
Intenta mantener el límite de tus líneas en 80 caracteres.Si es necesario, puedes dividir las líneas en varias e indentarlas, ya que PHP lo soporta perfectamente.Ganarás en facilidad de lectura y comprensión de tu código.
Declara las propiedades de las clases antes de los métodos.
Declara los métodos en este orden: public, protected y private.
A excepción de los constructores y los métodos setUp y tearDown de los tests PHPUnit que deben ir primero para mejorar la lectura.
Siempre que sean aplicables, usa el prefijo Abstract y los sufijos Interface, Trait y Exception.
Usa sólo una ‘instrucción’ por línea. (PSR-2) No uses los “;” para unir varias instrucciones.Incluso los if() más sencillos escríbelos en varias líneas.

```console
 // Haz esto:
 if (strlen($path) === 0) {
     return $this->getPathPrefix() ?: '';
 }

 // En lugar de esto:
 if (strlen($path) === 0) { return $this->getPathPrefix() ?: ''; }
```

Una excepción es el ‘operador condicional ternario’ a ? b : c que sí se puede usar en un sola línea o dividir en varias en caso de que las expresiones sean muy complejas, para facilitar su lectura.

```console
 $this->pathPrefix = $is_empty ? null : $prefix;
```

Los comentarios de una sola línea colócalos al mismo nivel que la línea a la que se refieren. (Como en el ejemplo anterior del ‘if’)
Elimina los espacios en blanco al final de las líneas y en las líneas en blanco. (PSR-2)Especialmente si usas algún sistema de versión de código, lo agradecerás.
Utiliza espacios para mejorar la lectura de los operadores:
Después del signo de negación !.

```console
if (! isset($config[$setting])) {
   continue;
}
```

Antes y después del signo igual “=”, de los operadores matemáticos y lógicos y de los signos del operador condicional ternario.

```console
public function setHost($host)
{
   $this->host = $host;

   return $this;
}
```

Usa comillas sencillas habitualmente y comillas dobles cuando quieras expandir una variable.
Usa los operadores lógicos && y || en lugar de AND y OR.
Usa una línea en blanco antes de los returns a no ser que sea la única línea dentro de una estructura. (Como un if)
Coloca los returns al comienzo de las funciones. (Return early)Especialmente en los casos en los que hagas validaciones con un return, hazlos al comienzo de la función. De ese modo es más fácil leer lo que hace la función y cuales son sus condiciones de salida.
No uses else para salir al final de las funciones.

```console
 // Haz esto
 public function getMimetype($path)
 {
     $path = Util::normalizePath($path);
     $this->assertPresent($path);

     if (! $object = $this->adapter->getMimetype($path)) {
         return false;
     }

     return $object['mimetype'];
 }

 // En lugar de esto
 public function getMimetype($path)
 {
     $path = Util::normalizePath($path);
     $this->assertPresent($path);

     if ($object = $this->adapter->getMimetype($path)) {
         return $object['mimetype'];
     } else {
         return false;
     }        
 }
```

```console
 // Haz esto
 public function getMimetype($path)
 {
     $path = Util::normalizePath($path);
     $this->assertPresent($path);
 
     if (! $object = $this->adapter->getMimetype($path)) {
         return false;
     }
 
     return $object['mimetype'];
 }
 
 // En lugar de esto
 public function getMimetype($path)
 {
     $path = Util::normalizePath($path);
     $this->assertPresent($path);
 
     if ($object = $this->adapter->getMimetype($path)) {
         return $object['mimetype'];
     } else {
         return false;
     }        
 }
 ```

Para los nombres de los métodos:Cuando un objeto tiene una relación principal con varias ‘cosas’, como objetos, parámetros, etc… se usan estos nombres:

* set()
* has()
* all()
* get()
* replace()
* remove()
* clear()
* isEmpty()
* add()
* register()
* count()
* keys()

Para relaciones a varios dónde la relación no sea principal, se aplican estos otros nombres:

Relación Principal	Otras Relaciones

* get()	getXXX()
* set()	setXXX()
* n/a	replaceXXX()
* has()	hasXXX()
* all()	getXXXs()
* replace()	setXXXs()
* remove()	removeXXX()
* clear()	clearXXX()
* isEmpty()	isEmptyXXX()
* add()	addXXX()
* register()	registerXXX()
* count()	countXXX()
* keys()	n/a

Aunque setXXX y replaceXXX se parecen, la diferencia es que mientras setXXX puede modificar o añadir elementos a la relación, replaceXXX no puede añadir elementos. Y si recibe una clave desconocida, debe lanzar una excepción.

Nombres de las rutas.Usa nombres en línea con las convenciones internas de Laravel:

* users.index
* users.create
* users.store
* users.show
* users.edit
* users.update
* users.destroy

Nombres de los modelos Eloquent.Laravel usa como convención para los modelos la notación StudlyCaps y para el nombre de la tabla relacionada con tu modelo, el nombre del modelo en minúsculas y plural.Por ejemplo, para class User extends Eloquent {}, Laravel buscará una tabla llamada users.Y como convención, usará como clave primaria un campo llamado id.Para los nombres de las columnas en la tabla, usa la notación snake_case. Y para los métodos de los modelos, usa camelCase. Por ejemplo, para una columna llamada nombre_completo, el método sería getNombreCompletoAttribute($name).Para las tablas pivots, el convenio es usar el singular de ambas tablas unidas por un guión bajo. Por ejemplo: user_product.
Otros tutoriales que te pueden interesar
