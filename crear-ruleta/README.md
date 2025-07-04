# Crear Ruleta

Al ingresar a esta sección, verás la siguiente visual:

<figure><img src="../.gitbook/assets/image (1).png" alt=""><figcaption><p>Figura #1: Captura de pantalla Creación de ruletas.</p></figcaption></figure>

Aquí podrás configurar los diferentes campos para personalizar tu ruleta. A continuación, se detallan las opciones disponibles:

* **Fecha inicial**: Especifica la fecha en la que la ruleta estará disponible para participar.
* **Fecha final**: Indica la fecha hasta la cual la ruleta permanecerá activa.
* **Nombre**: Asigna un nombre único a la ruleta.
* **Orden**: Define la posición de la ruleta en relación con otras disponibles.

{% hint style="info" %}
**Ejemplo**: Si se crean 2 ruletas.

* Ruleta X: Orden 2.
* Ruleta Y: Orden 1.

Se activará primero la ruleta 1, ya que tiene prioridad por su orden asignado.
{% endhint %}

* **Descripción**: Proporciona una breve descripción de la ruleta.
* **Usuario puede participar varias veces**: Indica si los usuarios podrán participar múltiples veces en la misma ruleta.
* **Fecha de expiración o días**: Al configurar este campo, estarás indicando la fecha máxima que tiene el usuario para activar la ruleta, esta será en fecha específica o en cantidad de días.
  * **Fecha**: Se habilitará el campo "**Fecha Expiración**", en el que debes agregar la fecha en la que expirará la ruleta.
  * **Días**: Se desplegará el campo "**Días**" en el que debes agregar la cantidad de días que estará habilitada la ruleta.
* ¿**Es para registro**?: La ruleta se asignará automáticamente solo a los usuarios nuevos de la plataforma.
  * **Si**: la configuración "¿**Es para inicio de sesión**?" desaparecerá del formulario y se asignará a los usuarios que realicen el registro en la plataforma.
  * **No**: La ruleta no se asignará por registro.
* ¿**Es para inicio de sesión**?: Debes indicar si la ruleta aparecerá por cada inicio de sesión en la plataforma.
  * Si: la configuración "¿**Es para registro**?" desaparecerá del formulario y se asignará automáticamente en el primer inicio de sesión del día para los usuarios configurados.
  * No: El usuario solo podrá activar la ruleta una vez y no podrá recibir giros adicionales.

{% hint style="warning" %}
**Nota**: Tener en cuenta que solo aparecerá en el primer inicio de sesión del día y si no tiene ruleta por registro asignada.
{% endhint %}

* **Pasarelas de pago**: Define si los usuarios pueden participar en la ruleta mediante ciertas pasarelas de pago o todas ellas.
* **Tipo de producto**: Establece con qué tipo de producto se activará la ruleta.

{% hint style="warning" %}
**Nota**: Si seleccionas "**Pasarelas de pago**" o "**Tipo Producto**", la otra opción se desactivará automáticamente, ya que la ruleta solo puede configurarse mediante una de estas alternativas.
{% endhint %}

La configuración "**Tipo de producto**" mostrará diferentes opciones dependiendo de la selección realizada. Para obtener más detalles sobre estas configuraciones, puedes hacer clic en el siguiente enlace:

{% content-ref url="broken-reference" %}
[Broken link](broken-reference)
{% endcontent-ref %}

A continuación, se describen las configuraciones estándar que permanecerán sin cambios, independientemente de las opciones seleccionadas anteriormente.

### Configuración de Moneda: <a href="#configuracion-moneda-ruleta" id="configuracion-moneda-ruleta"></a>

En este apartado verás la moneda correspondiente al país seleccionado antes de ingresar a torneos y bonos, al seleccionarla se desplegarán las siguientes configuraciones:

<figure><img src="../.gitbook/assets/image (1) (1).png" alt=""><figcaption><p>Figura #2: Captura de pantalla configuraciones moneda.</p></figcaption></figure>

Las opciones disponibles son las siguientes:

* **Valor mínimo de activación**: Define el monto mínimo necesario para activar la ruleta.
* **Máxima cantidad de giros diarios**: Establece el número máximo de giros que un usuario puede realizar por día.
* **Jugadores**: Especifica los usuarios que tendrán acceso a la ruleta, cargando un archivo [CSV](https://app.gitbook.com/o/QcwavWzh0dfIwPyknoIT/s/mbqa0WvDWam8G20QQoIZ/#csv) con los ID de los jugadores.

{% hint style="warning" %}
**Nota**: Para ver los ID´s de los jugadores ingresados, puedes utilizar el botón 👁️
{% endhint %}

### Tipo de Premio

En este apartado, deberás definir el tipo de premio que los usuarios podrán ganar al girar la ruleta. Dependiendo de la opción seleccionada, necesitarás configurar los siguientes campos:

* **Premio Físico**: Si el premio es un objeto físico, deberás configurar los siguientes campos:
  * **Descripción del premio**: Breve descripción del premio.
  * **URL de imagen de la ruleta**: Proporciona la URL de la imagen que representa la ruleta.
  * **URL de imagen del premio**: Proporciona la URL de la imagen del premio.
  * **Porcentaje**: Define la probabilidad de que un usuario gane este premio.
  * **Botón agregar**: Al hacer clic en este botón, el premio se añadirá a la ruleta.
* **Premio en Dinero**: Si el premio es un monto de dinero, deberás configurar los siguientes campos:
  * **URL de imagen de la ruleta**: Proporciona la URL de la imagen que representa la ruleta.
  * **URL de imagen del premio**: Proporciona la URL de la imagen del premio.
  * **Saldo asignado**: Especifica el tipo de saldo que recibirá el usuario.
  * **Monto**: Define el valor monetario que se asignará al usuario.
  * **Porcentaje**: Define la probabilidad de que un usuario gane este premio.
  * **Botón agregar**: Al hacer clic en este botón, el premio se añadirá a la ruleta.
* **Premio en Bono**: Si el premio es un bono, deberás configurar los siguientes campos:
  * **URL de imagen de la ruleta**: Proporciona la URL de la imagen que representa la ruleta.
  * **URL de imagen del premio**: Proporciona la URL de la imagen del premio.
  * **Saldo asignado**: Especifica el tipo de saldo que recibirá el usuario.
  * **Monto**: Define el valor del bono que se asignará al usuario.
  * **Porcentaje**: Define la probabilidad de que un usuario gane este premio.
  * **Botón agregar**: Al hacer clic en este botón, el premio se añadirá a la ruleta.
*   **Intenta nuevamente**: Esta opción añade un nuevo giro a la ruleta. Si al girarla cae en esta opción, el usuario podrá girar nuevamente sin salir de la interfaz de la ruleta.

    {% hint style="warning" %}
    **Nota**: Si la ruleta vuelve a caer en esta opción, se activará de manera instantánea y consecutivamente hasta que salga otro tipo de premio, adicional, si el usuario sale de la ruleta, este premio se perderá sin ser acumulable.
    {% endhint %}

    * **URL de imagen de la ruleta**: Proporciona la URL de la imagen que verá en la ruleta.
    * **URL de imagen del premio**: Proporciona la URL de la imagen que se verá si este premio queda seleccionado por la ruleta.
    * **Porcentaje**: Define la probabilidad de que un usuario gane este premio.
    *   **Botón agregar**: Al hacer clic en este botón, el premio se añadirá a la ruleta.

        {% hint style="warning" %}
        Nota: Se pueden agregar varios giros extras en una sola ruleta.
        {% endhint %}



{% hint style="warning" %}
**Nota**: La totalidad del porcentaje de los premios en la ruleta no debe exceder el 100%, en caso de exceder este valor, no permitirá agregar más premios.
{% endhint %}

#### Tabla de premios:

Los premios que se agreguen se podrán visualizar en una tabla con las siguientes columnas:

* **Tipo de premio**: Podrás evidenciar el tipo de premio agregado.
* **Descripción**: Podrás evidenciar una breve descripción del premio.
* **Tipo Saldo:** Podrás evidenciar el tipo de saldo del premio en caso de que aplique.
* **Bono valor**: Podrá evidenciar el monto del bono que tendrá el usuario con el premio en caso de que aplique.
* **URL imagen ruleta**: Podrás evidenciar la URL de la imagen que estará en la ruleta por este premio.
* **URL imagen premio**: Muestra la URL de la imagen del premio si ha sido seleccionado.
* **Porcentaje**: Indica la probabilidad de que el premio agregado sea obtenido.
* **Acción**: Permite eliminar el premio de la ruleta mediante un botón disponible.

#### Opciones Avanzadas

Al seleccionar "**Opciones avanzadas**", se desplegarán los siguientes campos:

<figure><img src="../.gitbook/assets/image (2).png" alt=""><figcaption><p>Figura #3: Captura de pantalla opciones avanzadas.</p></figcaption></figure>

* **URL de fondo**: Especifica la URL de la imagen de fondo que aparecerá en la ruleta.
* **Regiones Usuario**: Indica las regiones donde la ruleta estará disponible.
* **Departamentos Usuario**: Indica los departamentos donde la ruleta estará disponible.
* **Ciudades Usuario**: Indica las ciudades donde la ruleta estará disponible.

Una vez configurada la ruleta, haz clic en el botón **"Crear Ruleta"** para guardar los ajustes y crear la ruleta.

{% hint style="danger" %}
**Notas importantes**:&#x20;

* Los campos que finalizan el nombre con un \* son obligatorios para la creación de la ruleta.
* Las ruletas de casino y deportivas solo se activarán cuando la apuesta haya sido realizada con saldo real (Es decir, si la apuesta se realiza con un bono, la ruleta no se activará).
{% endhint %}
