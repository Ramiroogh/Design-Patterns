La idea de CQRS es separar la lógica de las consultas (recuperación de datos) y la de comandos (inserción actualización y borrador de datos)
+ esto producirá un alto rendimiento

recuperar


insertar actualizar borrar


De hecho, el patrón establece que no importa si combinamos una base de datos SQL con otra NoSQL.
Es incluso mejor, dado que las primeras son mas rapidas escribiendo, y las segundas leyendo informacion.

## Evitar Service BUS
Para evitar perdidas Del información, las bases de datos deben estar siempre sincronizadas entre sí a través de un Service Bus.
+ este puede ser una cola de mensajes como Kafka o rap rabbitMQ