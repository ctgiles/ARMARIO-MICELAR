### 21/10/24
- Adición de bibliotecas necesarias para tratar la tarjeta SD y el módulo RTC.
- Uso de pines relativos al protocolo SPI para conexión del lector de tarjeta SD.
- Adición de variables relativas a la tarjeta SD y el módulo RTC, incluidas intervalos de tiempo.
- Modificación del constructor "setup()" para que incluya la inicialización de los nuevos componentes.
- Adición de "String obtenerFechaHora(DateTime t)": función para crear string con la fecha y hora actuales.
- Adición de "void EnvioTarjetaSD()": función para enviar a la tarjeta SD los datos de los sensores y la fecha y hora en las que se han tomado.
- Actualización del bucle principal "void loop()" lara incluir estos cambios en el código.

### 13/10/2024
- Cambio pines sensores y botones para liberar pines de SPI (los necesitamos más adelante).
- Cambio pines y funciones relativas a control de temperatura.
- - Se eliminan calefactores y se reutilizan los pines para control de relays del nuevo sist. de refrigeración y calefacción.
  - Se elimina función "void TemperaturaBaja()".
  - Se renombra "void TemperaturaAlta()" como "void Ventilacion()".
  - Se añade función "void ActuadorTemperatura()", análoga a "void ActuadorHumedad()", para control de sist. de refrigeración y calefacción.
- Actualización del bucle principal "void loop()" para incluir estos cambios de funciones.
