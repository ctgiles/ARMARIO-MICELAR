### 13/10/2024
- Cambio pines sensores y botones para liberar pines de SPI (los necesitamos más adelante)
- Cambio pines y funciones relativas a control de temperatura.
- - Se eliminan calefactores y se reutilizan los pines para control de relays del nuevo sist. de refrigeración y calefacción.
  - Se elimina función "void TemperaturaBaja()".
  - Se renombra "void TemperaturaAlta()" como "void Ventilacion()".
  - Se añade función "void ActuadorTemperatura()", análoga a "void ActuadorHumedad()", para control de sist. de refrigeración y calefacción.
- Actualización del bucle principal "void loop" para incluir estos cambios de funciones.
