# dashboard deposito

## 1. Acceso al Módulo

**Ruta de Acceso**: Virtualsoft/ Informes compartidos/ Datas TI/ Qlik.

***

## 🖼️2. Visualización

<figure><img src=".gitbook/assets/image (2).png" alt=""><figcaption><p>Figura #1: Captura de pantalla dashboard.</p></figcaption></figure>

***

## 3. Funcionalidades

### 3.1 Resumen de Dashboard Deposito

El dashboard muestra KPIs generales de depósitos, gráficos de evolución diaria y mensual, comparativos por canal (pasarela vs punto de venta), rankings de usuarios y medios de pago, además de tablas detalladas y resúmenes por usuario. Toda la información se puede filtrar y exportar.

### 3.2 Filtros

| Campo             | Tipo de Control | Descripción                                                    | Validaciones                                                  |
| ----------------- | --------------- | -------------------------------------------------------------- | ------------------------------------------------------------- |
| `Partner`         | Dropdown        | Mostrará únicamente datos del partner elegido.                 | Solo se visualizarán los partners configurados en el reporte. |
| `País`            | Dropdown        | Las gráficas mostrarán solo datos del país elegido.            |                                                               |
| `Año`             | Dropdown        | Las gráficas mostrarán solo datos del año seleccionado.        |                                                               |
| `Mes`             | Dropdown        | Las gráficas solo reflejaran información del mes seleccionado. |                                                               |
| `Dia mes`         | Dropdown        | Las gráficas mostrarán solo el mes elegido.                    |                                                               |
| `Estado Deposito` | Dropdown        | **Filtra por estado del depósito.**                            |                                                               |

### 3.3 KPIs

| Nombre del campo    | Descripcción                                                  | Obervaciones                                                  |
| ------------------- | ------------------------------------------------------------- | ------------------------------------------------------------- |
| **Valor depósito**  |  Suma total de todos los primeros depósitos realizados.       | Este campo varía la información según los filtros utilizados. |
| **Cant. Depósitos** | Cantidad total de todos los primeros depósitos.               | Este campo varía la información según los filtros utilizados. |
| **Promedio Valor**  | Promedio de primeros depósitos realizados.                    | Este campo varía la información según los filtros utilizados. |
| **Cant. usuarios**  | Cantidad total de usuarios que realizaron un primer depósito. | Este campo varía la información según los filtros utilizados. |

### 3.4 Gráficas

| Gráfica                     | Descripcción                                                                             | Obervaciones          |
| --------------------------- | ---------------------------------------------------------------------------------------- | --------------------- |
| **Depósitos diarios**       | Gráfica con eje x monto total de los depósitos y eje y con día del depósito.             | Gráfica líneal.       |
| **Valor depósitos mensual** | Monto total de los depósitos mensuales y eje x con meses disponibles.                    | Gráficas tipo barras. |
| **Top % valor pasarela**    | Pasarelas de pago más utilizadas.                                                        | Gráfica tipo torta.   |
| **Top % valor punto venta** | Puntos de venta con mayor monto depositado.                                              | Gráfica tipo torta.   |
| **Medio del depósito**      | Comparación mensual entre pasarelas de pago y depósitos por puntos de venta (mismo mes). | Gráficos tipo barras. |
| **Top usuario**             | Usuarios con mayor valor depositado.                                                     | Gráficas tipo barras. |

### 3.5 Tablas

#### 3.5.1 Resumen usuario:&#x20;

| Id Usuario                                         | Valor\_Deposito                                        | Cantidad Deposito                              | Promedio depósito                            |
| -------------------------------------------------- | ------------------------------------------------------ | ---------------------------------------------- | -------------------------------------------- |
| Identificación de usuario que realizó el depósito. | Suma total de los depósitos realizados por el usuario. | Número de depósitos realizados por el usuario. | Promedio de valor depositado por el usuario. |

#### 3.5.2 Detalle depósitos:&#x20;

| Columna                   | Descripción                                              |
| ------------------------- | -------------------------------------------------------- |
| Id Usuario                | Identificación del usuario que realizó el depósito.      |
| Id Deposito               | Identificación del depósito realizado.                   |
| Id Externo                | Id externo de la transacción.                            |
| Fecha Creación depósito   | Fecha de la creación del depósito en formato dd/mm/aaaa. |
| Medio del depósito        | Medio por el que se realizó el depósito.                 |
| Nombre medio del depósito | Nombre del medio por el que se realizó el depósito.      |
| Proveedor                 | Proveedor con el que se realizó el depósito.             |
| Estado Deposito           | Estado en el que se encuentra el depósito.               |
| Valor\_Deposito           | Valor del depósito realizado.                            |

### 🕒 4. Control de Versiones

| Versión | Fecha      | Autor         | Cambios Realizados |
| ------- | ---------- | ------------- | ------------------ |
| 1.0     | 02/07/2025 | Ronald Pelaez | Documento inicial  |
