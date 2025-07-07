---
description: >-
  Un torneo es una competencia donde los usuarios compiten por premios. En esta
  sección encontrarás información detallada sobre los campos para su
  configuración.
---

# Crear Torneo

Para iniciar, debes utilizar la opción "**Crear Torneo**".

<figure><img src="../.gitbook/assets/image (17).png" alt=""><figcaption><p>Figura #1: Captura de pantalla opción crear Torneo.</p></figcaption></figure>

Al ingresar a esta sección tendrás la siguiente visual:&#x20;

<figure><img src="../.gitbook/assets/image (18).png" alt=""><figcaption><p>Figura #2: Captura de pantalla sección crear torneo.</p></figcaption></figure>

* **Fecha inicial**: Fecha en la que el Torneo va a iniciar.
* **Fecha final**: Fecha en la que finalizará el torneo.
* **Nombre**: Nombre que tendrá el torneo.
* **Orden**: Orden de prioridad que tendrá el torneo para ser reclamado por el usuario.

{% hint style="info" %}
**Ejemplo**: Si tienes tres torneos con los siguientes valores de orden:

* **Torneo A**: Orden 1
* **Torneo B**: Orden 2
* **Torneo C**: Orden 3

Para reclamar el premio del Torneo C, primero debes completar y reclamar los premios del Torneo A y luego del Torneo B.
{% endhint %}

* **Descripción**: Descripción breve del torneo.
* **Tipo**: Indica si el torneo será público o privado.
  * **Público**: El torneo será abierto para todos los jugadores.
  * **Privado**: El torneo será para usuarios VIP, al seleccionar esta opción se desplegará un campo llamado "**Jugadores**" en el cuál debes ingresar los jugadores que tendrán acceso al torneo por medio de un archivo [CSV](https://app.gitbook.com/o/QcwavWzh0dfIwPyknoIT/s/mbqa0WvDWam8G20QQoIZ/#dashboard).
* **Visible para todos los jugadores**: Debes establecer si el torneo podrá ser visto por todos los jugadores.
* **Tipo Producto:** Define los productos con los que el usuario podrá sumar puntos en el torneo. Es posible seleccionar múltiples opciones, pero con restricciones:
  * [**Sportsbook**](https://app.gitbook.com/o/QcwavWzh0dfIwPyknoIT/s/mbqa0WvDWam8G20QQoIZ/#sportsbook) puede combinarse con cualquiera de las otras opciones.
  * **Casino, Casino en Vivo y Virtuales** no pueden combinarse entre sí.

{% hint style="info" %}
**Ejemplo**: Puedes seleccionar **Sportsbook + Casino** o **Sportsbook + Virtuales**, pero no **Casino + Virtuales**.
{% endhint %}

Esta configuración altera ciertos campos, para obtener información sobre los campos correspondientes a las opciones que tomes en **tipo de producto**, puedes dar clic en la siguiente página:

{% content-ref url="broken-reference" %}
[Broken link](broken-reference)
{% endcontent-ref %}

A continuación, se presentan las configuraciones estándar que no varían según ajustes previos:

* **Tipo de Ranking**: Indica por qué tipo de ranking se va a regir el torneo, ciertas opciones desplegarán otras configuraciones.
  * **Ganancia neta**: El ranking de torneo será regido solo por las ganancias registradas (Si seleccionas esta opción no se desplegarán las configuraciones de[#ranking](./#ranking "mention")).
    * **Valor punto**: Debes especificar el valor de cada punto que recibirá el usuario por ganancias en apuestas.&#x20;
  * **Monto Dinero**: El ranking del torneo será regido por dinero acumulado.
  * **Líneas de apuestas**: El ranking del torneo será regido por la cantidad de líneas de apuestas realizadas.
* **Multiplicar líneas por puntos**: Esta configuración se utiliza para la sección de deportivas, en la cual se debe indicar si se multiplican los puntos por cada línea de apuesta.
* **Todas las condiciones son obligatorias**: Debes indicar si se deben cumplir todas las condiciones configuradas por el bono, para que el usuario sume puntos.

### Moneda

&#x20;Al seleccionar la moneda correspondiente al país para el que se está configurando el torneo, se desplegarán las siguientes configuraciones:

<figure><img src="../.gitbook/assets/image (19).png" alt=""><figcaption><p>Figura #3: Captura de pantalla Moneda.</p></figcaption></figure>

* **Mínimo valor de la apuesta**: En este campo debes indicar el monto mínimo que se debe apostar para poder sumar puntos en el torneo.
* **Tipo de Premio:** Desde esta configuración podrás seleccionar el tipo de premio que otorgará el torneo, teniendo en cuenta que cada opción desplegará ciertas configuraciones, las cuales son las siguientes:
  * **Físico**: Estarás indicando que el premio del torneo será físico, por lo que es necesario configurar los siguientes campos:
    * **Posición**: Indica la posición en la cual se asignará el premio en la tabla de premiaciones.
    * **Descripción premio**: Especifica una breve descripción del premio, la cual será visible para el usuario en la plataforma.
    * **URL Imagen Premio**: Debes agregar la URL correspondiente a la imagen del premio. Para agregar otro premio, debes dar clic en el botón "**Agregar**".
    * **Importar CSV**: En este campo debes ingresar un archivo [CSV](https://app.gitbook.com/o/QcwavWzh0dfIwPyknoIT/s/mbqa0WvDWam8G20QQoIZ/#dashboard) con la posición, el tipo de premio (Premio físico = 0), la descripción y la URL de la imagen.
  * **Dinero**: Estarás indicando que el premio del torneo será dinero, por lo que es necesario configurar los siguientes campos:
    * **Posición**: Indica la posición en la cual se asignará el premio en la taba de premiaciones.
    * **Saldo a asignar**: Tendrás las siguientes opciones para indicar el tipo de saldo que se asignará al usuario por el torneo:
      * Saldo créditos.
      * Saldo Premio.&#x20;
      * Saldo bono.
    * **Monto Premio**: Debes agregar el monto del premio. Para agregar otro monto, debes dar clic en el botón "**Agregar**".
    * **Importar CSV**: En este campo debes ingresar un archivo [CSV](https://app.gitbook.com/o/QcwavWzh0dfIwPyknoIT/s/mbqa0WvDWam8G20QQoIZ/#dashboard) con la posición, el tipo de premio (Dinero = 1), el tipo de saldo y el valor.
  * **Bono**: Al seleccionar esta opción, estarás indicando que el premio del torneo será en bonos, por lo que es necesario configurar los siguientes campos:
    * **Posición**: Indica la posición en la cual se asignará el premio en la taba de premiaciones.
    * **Asignación de bono**: En este campo debes asignar un bono previamente creado.
    * **Importar CSV**: Debes agregar un archivo CSV indicando la posición y la asignación del bono

### Ranking

En este apartado debemos configurar el rango de puntos según las apuestas realizadas en el torneo. Si un usuario realiza una apuesta dentro del rango establecido, sumará una cantidad específica de puntos.

En este apartado encontrarás los siguientes campos:

* **Rango inicial:** Ingresa el monto mínimo apostado a partir del cual se empezarán a otorgar puntos.
* **Rango final:** Especifica el monto máximo apostado que delimita el final del rango.
* **Puntos:** Define cuántos puntos recibirá el usuario por apostar un monto que se encuentre dentro de este rango.

Para agregar más rangos, debes dar clic en el botón "**Agregar**".

### Opciones avanzadas.

Como opciones avanzadas tendrás las siguientes configuraciones:

<figure><img src="../.gitbook/assets/image (20).png" alt=""><figcaption><p>Figura #4: Captura de pantalla opciones avanzadas.</p></figcaption></figure>

* **Código Global:** Debes ingresar un código configurado desde el BackOffice. Este código estará asociado al bono y tendrá un límite máximo de usuarios.
* **URL imagen principal:** Ingresa la URL de la imagen principal del torneo. Esta imagen será visible para todos los usuarios.
* **Máximo de jugadores:** Especifica la cantidad máxima de jugadores que podrán participar en el torneo.
* **Mínimo de jugadores:** Define la cantidad mínima de jugadores requerida para que el torneo pueda iniciar.
* **Regiones de usuario:** Indica las regiones en las que el torneo estará disponible.
* **Departamentos de usuario:** Especifica los departamentos donde se habilitará el torneo.
* **Ciudades de usuario:** Define las ciudades en las que el torneo estará disponible.
* **URL fondo:** Ingresa la URL de la imagen que se utilizará como fondo para el torneo.
* **URL imagen central:** Especifica la URL de la imagen central del torneo.
* **URL imagen derecha:** Ingresa la URL de la imagen que se mostrará en el lado derecho del torneo.
* **URL fondo detallado:** Proporciona la URL del fondo interno del torneo.
* **URL imagen central detallada:** Especifica la URL de la imagen central detallada del torneo.
* **URL imagen premios:** Ingresa la URL de la imagen que representará los premios del torneo.

Una vez que hayas completado todos los campos y configuraciones del torneo, para finalizar el proceso debes dar clic en el botón **"Crear Torneo"**. Esto guardará la configuración y activará el torneo para los usuarios.

{% hint style="warning" %}
**Nota**: Los campos que finalizan el nombre con un \* son obligatorios para la creación del torneo.
{% endhint %}
