---
description: >-
  Este módulo permite gestionar tus wallets cripto asociadas a una criptomoneda
  y red específica.
---

# Wallets Crypto

## 1. Acceso al Módulo

**Ruta de Acceso**: menú > Servicios > Gestión > Wallets Crypto.

***

## 2. 🖼️ Visualización

<figure><img src=".gitbook/assets/image (6).png" alt=""><figcaption><p>Figura #1: Captura de pantalla Wallets Crypto.</p></figcaption></figure>

## 3. Funcionalidades

### &#x20;2.1. 🔢 Resumen de Wallets Crypto&#x20;

Aquí podrás registrar, visualizar y eliminar direcciones de Wallets Crypto vinculadas a tu cuenta. Estas direcciones serán utilizadas para retiros con tipo "Criptomonedas".

#### 2.1.1. Formulario para crear Wallets Crypto:

| Campo.                     | Descripción.                                              | Observaciones.                                                 |
| -------------------------- | --------------------------------------------------------- | -------------------------------------------------------------- |
| Crypto Monedas             | Selecciona una cripto moneda creada previamente.          |                                                                |
| Red Blockchain             | Red asociada a la criptomoneda (ej: TRC20, ERC20, BEP20). | Debe coincidir con la red de destino, según el tipo de cripto. |
| Dirección Wallet           | Dirección cripto a la que se enviarán los fondos.         | Verifica que sea válida y compatible con la red seleccionada.  |
| Confirmar Dirección Wallet | Reingresa la dirección para asegurar que sea correcta.    | Ambas direcciones deben coincidir para habilitar el registro.  |

2.1.2. **📊 Tabla de Wallets Registradas.**

| Campo.           | Descripción.                                                                  |
| ---------------- | ----------------------------------------------------------------------------- |
| Criptomoneda     | Muestra la criptomoneda asociada a la wallet registrada.                      |
| Red Blockchain   | Indica la red seleccionada al momento del registro de la wallet.              |
| Dirección Wallet | Dirección cripto registrada. Se visualiza en formato abreviado por seguridad. |
| Estado           | Indica si la wallet está activa para realizar retiros o ha sido desactivada.  |

#### 2.1.3. Acciones del usuario.

<table><thead><tr><th width="158.09088134765625">Icono</th><th>Acción</th><th>Descripción</th></tr></thead><tbody><tr><td><div><figure><img src=".gitbook/assets/image (7).png" alt="" width="188"><figcaption></figcaption></figure></div></td><td>Guardar</td><td>Permite registrar una nueva wallet cripto.</td></tr><tr><td><div><figure><img src=".gitbook/assets/image (8).png" alt=""><figcaption></figcaption></figure></div></td><td>Eliminar</td><td>Elimina de forma permanente la wallet cripto registrada. Solo disponible si la wallet está activa. Se solicita confirmación antes de ejecutar la acción.</td></tr></tbody></table>

***

### 3.✅ Validaciones y Reglas de Negocio

* Solo se pueden registrar wallets de criptomonedas previamente configuradas en BackOffice.
* Es obligatorio seleccionar correctamente la red blockchain asociada a la criptomoneda (por ejemplo: USDT en TRC20 o ERC20).
* Si no hay wallets activas registradas, no será posible solicitar retiros con tipo “Criptomonedas”.
* No se permite registrar múltiples wallets con la misma dirección y red.

***

### 3.📘 Glosario de Términos

| Término              | Definición                                                                                                                                                |
| -------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **Wallet Cripto**    | Billetera digital que permite recibir y almacenar criptomonedas. Funciona como una cuenta de destino en retiros.                                          |
| **Dirección Wallet** | Código alfanumérico único que identifica tu wallet en una red blockchain. Similar a un número de cuenta bancaria.                                         |
| **Criptomoneda**     | Activo digital descentralizado que utiliza criptografía para operar, como USDT, BTC o ETH.                                                                |
| **Red Blockchain**   | Infraestructura tecnológica por la que se transfiere una criptomoneda. Ejemplos: TRC20, ERC20, BEP20. Es fundamental que coincida con la red del destino. |
| **Estado Activo**    | Indica que una wallet está habilitada para ser usada en retiros.                                                                                          |
| **Estado Inactivo**  | La wallet ha sido deshabilitada y no puede ser seleccionada para retiros.                                                                                 |
