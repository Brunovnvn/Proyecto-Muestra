# Proyecto-Muestra

Dron terreste de 2 ruedas motorizadas +  1 rueda con libre sentido
Controlado por modulo BLE (Blootooth Low Energy) que a su vez esta conectado a microcontrolador (Raspberry Pi-Pico)
Conectado a aplicación movil (MIT App Inventor)
Control de ambos motores por medio de un rele (DPDT - MR62-N3 (Bobina 5V) )
Codigo de programa creado en Visual Studio
Desarrollo del circuito en software KiCad

Permite el control de:
  - Luces
  - Bocina
  - Direccion de dron
  - Velocidad de dron
  - Sensor instalado
  - Conexion y desconexion de modulo BLE

Información de microcontrolador:
  Pines PWM (Velocidad de ambos motores):
    - 4 (Motor 1 - Izq) y 5 (Motor 2 - Der)
  Pines PWM (Direccion de ambos motores):
    - 9 (Motor 1 - Izq) y 10 (Motor 2 - Der)
  Pines UART0 (BLE):
    - 1 y 2
  Pines control de luces:
    - 
  Pines sensor:
    - 
  Pin bocina:
    - 15
  
  
Alimentación de placa:
  - 5V
  - Cable naranja (Positivo +)
  - Cable azul (Negativo -)

Componentes usados: 
  - (2x) Transistor (Bipolar) BC337
  - (2x) Relé (DPDT - MR62-N3 (Bobina 5V) )
  - (2x) Resistencia 220 Ohms
  - (2x) Transistor (NPN) 
  
Precauciones: !!!!!!!
  - Autoiuducción de relé / Solución: Diodo
  - En cada cambio de direccion, 
  apagar PWM por unos milisegundos 
  para no producir un arco
      
