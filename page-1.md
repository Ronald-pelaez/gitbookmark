# Page 1

## Retirar

### 1. Acceso al Módulo

**Ruta de Acceso**: Menú > Gestión > Retirar

***

### 2. Visualización

Al acceder al módulo, el jugador encontrará dos opciones principales:

* **Solicitar retiro**
* **Consultar histórico**

#### 2.1 Solicitar retiro

Al hacer clic en **Seleccionar retiro**, se muestra información relevante. El jugador debe confirmarla para continuar.

Luego podrá seleccionar el **Tipo de Retiro** (ej. Transferencia, Criptomonedas, etc.) e ingresar el monto a retirar.

{% hint style="warning" %}
**Nota**: Para que se habilite el botón continuar, primero debes seleccionar el tipo de retiro.
{% endhint %}

Después de ingresar los datos, se muestra una pantalla de confirmación:

Al hacer clic en "**Crear retiro**", se genera la nota de retiro correspondiente.

#### 2.2 Retiro con Criptomonedas

Al seleccionar **Criptomonedas** como tipo de retiro:

* El campo “**Cuenta bancaria**” se reemplaza por **Wallet registrada**.
* Se muestra una lista con las wallets activas del jugador en el siguiente formato:

📌 Si no hay wallets activas:

> “No tienes wallets activas registradas para realizar retiros. Agrega una desde tu perfil.”

**Campos mostrados al jugador**

| Campo           | Tipo           | Obligatorio | Descripción                     |
| --------------- | -------------- | ----------- | ------------------------------- |
| Monto a retirar | Campo numérico | Sí          | Valor en moneda local (ej: PEN) |

{% hint style="warning" %}
Nota: La conversión a cripto se calcula en el momento del pago, no se muestra en pantalla.
{% endhint %}

***

#### 2.3 Consultar histórico

Desde el botón **Consultar histórico**, el jugador accede al registro de sus retiros.

Permite:

* Filtrar por fecha y estado
* Visualizar información clave de cada nota
* Acceder a juegos desde esta sección

**Retiros cripto en historial**

* Columna **Tipo**: muestra "Criptomoneda"
* Nuevas columnas al momento del pago:

| Columna nueva   | Descripción                                                 |
| --------------- | ----------------------------------------------------------- |
| TRM utilizada   | Tasa de conversión aplicada según proveedor o configuración |
| Monto en cripto | Valor resultante de la conversión al momento del pago       |

***

### 3. Validaciones y Reglas de Negocio

#### 3.1 Validaciones al confirmar solicitud

| Validación           | Mensaje de error                                        |
| -------------------- | ------------------------------------------------------- |
| No seleccionó wallet | “Ingresa todos los campos requeridos.”                  |
| Monto vacío          | “Ingresa todos los campos requeridos.”                  |
| Valor fuera de rango | “Valor menor al mínimo permitido para retirar."         |
| Fondos insuficientes | “No tienes saldo suficiente para realizar este retiro.” |

#### 3.2 Datos registrados

| Dato                  | Fuente                                 |
| --------------------- | -------------------------------------- |
| Criptomoneda / Red    | Desde la wallet seleccionada           |
| Wallet destino        | Seleccionada desde la lista de wallets |
| Monto en moneda local | Ingresado por el jugador               |
| Estado inicial        | Activo                                 |
| Fecha y hora          | Automática                             |

***

### 4. Anulación de retiros

El botón **Anular** estará disponible **solo si el retiro está en estado Activo**.

| Estado del retiro | ¿Botón visible? |
| ----------------- | --------------- |
| Activo            | ✅ Sí            |
| Pendiente Manual  | ❌ No            |
| Pendiente Sistema | ❌ No            |
| Pagado            | ❌ No            |
| Anulado           | ❌ No            |

Al hacer clic, se muestra:

> “¿Estás seguro que deseas eliminar la nota de retiro + (número de nota)?”

Si se confirma:

* El estado del retiro cambia a **Anulado**
* Se registra la acción en auditoría

***

### 5. Control de Accesos

| Acción                   | Requisito                       |
| ------------------------ | ------------------------------- |
| Ver opción Criptomonedas | Jugador con retiros habilitados |
| Confirmar retiro         | Jugador logueado y activo       |
| Anular nota              | Solo si el retiro está “Activo” |

***

### 6. Glosario

| Término           | Definición                                                            |
| ----------------- | --------------------------------------------------------------------- |
| **Estado Activo** | Solicitud generada por el jugador, aún no gestionada por un operador. |
| **Wallet Cripto** | Dirección registrada por el jugador para recibir retiros cripto.      |
| **TRM**           | Tasa de conversión cripto ↔ fiat aplicada al momento de pago.         |

***

### 7. Control de Versiones

| Versión | Fecha      | Autor         | Cambios Realizados                                                      |
| ------- | ---------- | ------------- | ----------------------------------------------------------------------- |
| 1.0     | --/--/---- | Virtualsoft   | Documento inicial                                                       |
| 1.1     | 07/07/2025 | Ronald Pelaez | Se agrega funcionalidad de retiro con criptomonedas y se aplica formato |
