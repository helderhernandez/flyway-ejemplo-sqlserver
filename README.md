# Información del proyecto base
Se tomo el *proyecto base* del siguiente ejemplo compartido en el tutorial de YouTube [Evolución de bases de datos con Flyway
](https://www.youtube.com/watch?v=8E54DaLKEFc) (código alojado en [Box](https://app.box.com/s/ieyfq3sd2wp3mc8wchc9pet67m0vgiys).)

# Requerimientos
Antes de poder ejecutar flyway, debera de:
- Crear la base de datos, verifique que haya conexión (que el puerto este libre, que no haya bloqueo por el firewall).
- Poseer credenciales de usuario con los permisos suficientes para poder generar consultas de DDL y DML.

Recuerde agregar la cadena de conexón y las credenciales al archivo de propiedades.

## Sobre las migraciones
Los scripts de actualización deben de colocarse en la folder de *migrations* (se proporcionan scripts de ejemplo).