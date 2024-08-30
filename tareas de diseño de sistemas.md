# Identificación de Modelos en Sistemas Reales: Sistema de Parqueadero ETITC

## Descripción del Modelo
El **Sistema de Parqueadero Automatizado** en la ETITC está diseñado para controlar el acceso y la salida de vehículos mediante  el reconocimiento de matrículas y carnets, optimizando el flujo de vehículos y mejorando la seguridad.

## Clases Identificadas
### Vehiculo
- **Atributos:**
  - `matricula`: String
  - `tipoVehiculo`: String
  - `propietario`: Usuario
- **Métodos:**
  - `identificarVehiculo()`
  - `registrarEntrada()`

### Usuario
- **Atributos:**
  - `nombre`: String
  - `idUsuario`: Integer
  - `carnetEstudiantil`: String
- **Métodos:**
  - `verificarAcceso()`
  - `registrarSalida()`

### Parqueadero
- **Atributos:**
  - `capacidadMaxima`: Integer
  - `ocupacionActual`: Integer
  - `vehiculosEstacionados`: List<Vehiculo>
- **Métodos:**
  - `actualizarOcupacion()`
  - `permitirAcceso(Vehiculo vehiculo)`

## Relaciones entre Clases
- Un **Usuario** tiene un **Vehiculo** asociado que es identificado por su **matricula**.
- El **Parqueadero** gestiona la entrada y salida de los **Vehiculos** y ajusta su **ocupacionActual** según el flujo de autos.
## UML
[![primero.png](https://i.postimg.cc/q7BFtszt/primero.png)](https://postimg.cc/qNYwSCc0)
# Problemas Comunes en el Diseño de Software


# Caso de Estudio: Sistema de Parqueadero Automatizado

### Problemas de Diseño Identificados
1. **Dependencia de la Tecnología:**
   - El sistema puede fallar si hay un problema con el reconocimiento , lo que puede causar demoras en la entrada y salida de vehículos.

2. **Capacidad Insuficiente:**
   - Si la capacidad del parqueadero no se ajusta a la demanda real, el sistema podría causar congestiones en lugar de prevenirlas.

3. **Seguridad de Datos:**
   - El manejo inadecuado de los datos de los usuarios y vehículos podría llevar a problemas de seguridad.

### Soluciones Alternativas
1. **Redundancia en los Sistemas:**
   - Implementar un sistema de respaldo manual o alternativas en caso de fallo tecnológico.

2. **Monitoreo en Tiempo Real:**
   - Integrar un sistema que ajuste a la ocupación y notifique cuando se esté acercando al límite de capacidad.

3. **Cifrado de Datos:**
   - Asegurar que todos los datos de los usuarios y vehículos estén encriptados y protegidos contra accesos no autorizados.

## Reflexión
Es crucial anticipar y acabar estos problemas desde la fase de diseño para asegurar la eficiencia y seguridad del sistema automatizado de parqueadero.

# Diseño de un Sistema de Información: Parqueadero ETITC

## Descripción del Sistema
El sistema automatizado para el parqueadero ETITC permite el acceso y salida de vehículos utilizando reconocimiento.

## Clases Definidas
### Vehiculo
- **Atributos:**
  - `matricula`: String
  - `tipoVehiculo`: String
  - `propietario`: Usuario
- **Métodos:**
  - `identificarVehiculo()`
  - `registrarEntrada()`

### Usuario
- **Atributos:**
  - `nombre`: String
  - `idUsuario`: Integer
  - `carnetEstudiantil`: String
- **Métodos:**
  - `verificarAcceso()`
  - `registrarSalida()`

### Parqueadero
- **Atributos:**
  - `capacidadMaxima`: Integer
  - `ocupacionActual`: Integer
  - `vehiculosEstacionados`: List<Vehiculo>
- **Métodos:**
  - `actualizarOcupacion()`
  - `permitirAcceso(Vehiculo vehiculo)`

## Interacción entre Clases
El **Usuario** utiliza su **Vehiculo** para ingresar al **Parqueadero**. El parqueadero verifica el acceso y ajusta la ocupación según el flujo de vehículos.
## UML
[![primero.png](https://i.postimg.cc/q7BFtszt/primero.png)](https://postimg.cc/qNYwSCc0)


# Análisis y Diseño de un Sistema: Parqueadero ETITC

## Descripción del Sistema
El sistema de parqueadero automatizado gestiona el acceso y salida del parqueadero en la ETITC utilizando tecnologías.

## Clases Definidas
### Vehiculo
- **Atributos:**
  - `matricula`: String
  - `tipoVehiculo`: String
  - `propietario`: Usuario
- **Métodos:**
  - `identificarVehiculo()`
  - `registrarEntrada()`

### Usuario
- **Atributos:**
  - `nombre`: String
  - `idUsuario`: Integer
  - `carnetEstudiantil`: String
- **Métodos:**
  - `verificarAcceso()`
  - `registrarSalida()`

### Parqueadero
- **Atributos:**
  - `capacidadMaxima`: Integer
  - `ocupacionActual`: Integer
  - `vehiculosEstacionados`: List<Vehiculo>
- **Métodos:**
  - `actualizarOcupacion()`
  - `permitirAcceso(Vehiculo vehiculo)`

## UML
[![primero.png](https://i.postimg.cc/q7BFtszt/primero.png)](https://postimg.cc/qNYwSCc0)

## Relaciones entre Clases
El sistema permite que un **Usuario** acceda al **Parqueadero** utilizando su **Vehiculo**, ajustando dinámicamente la **ocupacionActual** del parqueadero.

