# Información del proyecto base
Se tomo el *proyecto base* del siguiente ejemplo compartido en el tutorial de YouTube [Evolución de bases de datos con Flyway
](https://www.youtube.com/watch?v=8E54DaLKEFc) de NicoPaez, código original alojado en [Box](https://app.box.com/s/ieyfq3sd2wp3mc8wchc9pet67m0vgiys).

# Requerimientos
- Tener instalado Maven (para la gestión de dependencias).
- Crear la base de datos en SQL Server, verifique la conexión a su base de datos (a veces el puerto o las reglas del firewall obstaculizan la conexión).
- Poseer un usuario en la base de datos con los permisos suficientes para poder generar consultas de DDL y DML.

# Archivo de propiedades
Se proporciona un archivo ejemplo *flyway.properties.sample*, **copie** este archivo y renombre como **flyway.properties**, en el configure la cadena de conexón y las credenciales de usuario de la base de datos.

# Scripts SQL de migraciones
Los scripts SQL de actualización deben de colocarse en la folder de *migrations* (se proporcionan scripts de ejemplo).

Se recomienda crear folders para agrupar los script (esto con la finalidad de no acumular todos los scripts en el folder de migraciones).

# Comandos flyway

```bash
// para ver el estado actual de las migraciones
mvn flyway:info

// para realizar las migraciones
mvn flyway:migrate
```